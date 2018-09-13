# 水平垂直居中

## 仅居中元素定宽高适用：
- [absolute + 负margin](http://yanhaijing.com/vertical-center/absolute1.html)
- [absolute + margin auto](http://yanhaijing.com/vertical-center/absolute2.html)
- [absolute + calc](http://yanhaijing.com/vertical-center/absolute3.html)

## 居中元素不定宽高适用：
- [absolute + transform](http://yanhaijing.com/vertical-center/absolute4.html)
- [writing-mode](http://yanhaijing.com/vertical-center/writing-mode.html)
- [lineheight](http://yanhaijing.com/vertical-center/lineheight.html)
- [table](http://yanhaijing.com/vertical-center/table.html)
- [css-table](http://yanhaijing.com/vertical-center/css-table.html)
- [flex](http://yanhaijing.com/vertical-center/flex.html)
- [grid](http://yanhaijing.com/vertical-center/grid.html)

## 总结

下面对比下各个方式的优缺点，肯定又双叒叕该有同学说回字的写法了，简单总结下

- PC端有兼容性要求，宽高固定，推荐absolute + 负margin
- PC端有兼容要求，宽高不固定，推荐css-table
- PC端无兼容性要求，推荐flex
- 移动端推荐使用flex

**小贴士：**关于flex的兼容性决方案，请看这里《[移动端flex布局实战](//yanhaijing.com/css/2016/08/21/flex-practice-on-mobile/)》

| 方法                     | 居中元素定宽高固定 | PC兼容性                        | 移动端兼容性          |
| ---------------------- | --------- | ---------------------------- | --------------- |
| absolute + 负margin     | 是         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| absolute + margin auto | 是         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| absolute + calc        | 是         | ie9+, chrome19+, firefox4+   | 安卓4.4+, iOS6+   |
| absolute + transform   | 否         | ie9+, chrome4+, firefox3.5+  | 安卓3+, iOS6+     |
| writing-mode           | 否         | ie6+, chrome4+, firefox3.5+  | 安卓2.3+, iOS5.1+ |
| lineheight             | 否         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| table                  | 否         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| css-table              | 否         | ie8+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| flex                   | 否         | ie10+, chrome4+, firefox2+   | 安卓2.3+, iOS6+   |
| grid                   | 否         | ie10+, chrome57+, firefox52+ | 安卓6+, iOS10.3+  |


## 相关博文
http://yanhaijing.com/css/2018/01/17/horizontal-vertical-center/

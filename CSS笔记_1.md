# CSS笔记

## CSS导入

写多个CSS文件，分别负责不同的部分。eg:font.css, color.css ...

然后写一个basic.css 在basic中导入这些样式

    import url("font.css");
    import url("color.css");

在index.html中直接link一个css文件就可以了~~~

## CSS控制文本对齐方式

![CSS控制文本样式](img/CSS文本对齐方式.jpg)

vertical-align:可以设置元素的垂直对齐方式。其他值：middle,bottom...

line-height:设置行高，如果行高设置为height的高度，那么内部元素会垂直居中。可应用于输入框。

## CSS文字样式

![CSS文字样式](img/CSS文字样式.jpg)

## 可以使用!important提高样式的优先级。

    eg:color: red !important;

## CSS控制链接，鼠标移上、点击，移开...

![CSS控制链接](img/CSS控制链接.jpg)

注意：如果设置链接样式之后，点击过一次就不再起作用了 ---> 修改样式的顺序为L(点击之前)-V(访问之后)-H(鼠标放上)-A(点击的时候)。

**自定义链接样式：**

格式：
a:类名:状态名{样式...}

    a:web:visited {color:back}

### **其他伪类foscus**

可用于定义获取到焦点时的样式，如输入框.

    格式：selector:focus {样式}
    input:focus{
                background:gold;  
    }
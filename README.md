# modularLayoutDevelopment

1. icon图表
    <link href="图片路径.ico" rel="shortcut icon" />
    shortcut  icon中间有一个空格而不是一点'.'

2. 子元素浮动、父级清浮动(clear)

3. 模块化布局：先找出公共的样式，再写私有的样式。

4. css3解决渐变（不兼容） 让兼容浏览器使用css3渐变  不兼容的浏览器使用图片渐变

5. firefox内核前缀 chrome内核前缀
    css渐变设置  第一个参数 渐变方向
                第二个参数 初始颜色
                第三个参数 结束颜色
    background: -moz-linear-gradient(top, #f00, #00f);

6. chrome的内核  webkit
   firefox的内核  moz
   ie的内核       ms  ie9支持滤镜
   ie css3渐变写法 startColorstr endColorstr 不识别十六进制的简写，需要写全 #ff0000 gradientType=1代表横向渐变，gradientType=0代表纵向淅变
    filter: "progid:DXImageTransform.Microsoft.gradient(gradientType=0, startColorstr=#ff0000, endColorstr=#0000ff)";/*IE<9>*/
    -ms-filter: "progid:DXImageTransform.Microsoft.gradient(gradientType=0, startColorstr=#ff0000, endColorstr=#0000ff)";/*IE8+*/

7. CSS hack的目的就是使你的CSS代码兼容不同的浏览器。当然，我们也可以反过来利用CSS hack为不同版本的浏览器定制编写不同的CSS效果

8. ie6, 7, 8不支持圆角

9. 图片加圆角 需要再加上overflow:hidden  溢出的隐藏掉才能出现圆角

10. a标签与兄弟div之间默认有间隙; 去除间隙的方法是给a div共同的父标签添加font-size: 0;即可消除

11. div做成input效果
        <div class="search_input" contenteditable placeholder="六一儿童节快乐"></div>
        .search_input:empty::before {
            color:#9c9c9c;
            content:attr(placeholder);
        }

12. 去掉input聚焦时的蓝色边框 outline:none;

13. box-shadow:
    text-shadow  文字阴影

14. css绘制三角形 transparent 透明度
    ie6下将transparent改为#fff;



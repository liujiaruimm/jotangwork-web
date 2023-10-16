# css

css的引入方式

- 内嵌式：写在style的标签里，通常约定写在head标签里【小案例】
- 外联式：写在一个单独的.css文件中【通过link标签在网页中引入】【项目】
- 行内式：css写在标签的style属性中【但要配合java】



选择器

- 标签选择器【选中所有这个标签都生效】
- 类选择器【不以数字和中划线开头】
- 通配选择器



字体样式

- 字体大小font-size     数值+px
- 字体粗细font-weight
- 字体样式font-style
- 字体类型font-family





文本样式

- 文本缩进：text-indent【数值+px/em】em指一个字的大小
- 文本水平对齐方式：text-align

left 左对齐

center 居中对齐

right 右对齐



- 文本修饰：text-decoration
- underline下划线
- line-through删除线
- overline上划线
- none无装饰线



行高line-height  

-  +px
- 直接写数字【指字号的倍数】



设计行高和字体的连写方式

font：style weight size/line-height family



选择器的进阶：

- 复合选择器1.后代选择器：空格

                 2.子代选择器

- 并集选择器
- 交集选择器
- hover伪类选择器
- emmet语法



背景图平铺：background-repeat【简写bgr】

背景位置：1.方位名词 a.left center right

                            b.top center bottom

             2.数字+px【以盒子左上角为坐标原点】

第一个表示水平，第二个表示垂直

背景相关属性的连写bg：color image repeat position[不分先后顺序]



元素显示模式

- 块级模式：独占一行：div p h ul li dl dt dd form header nav footer
- 行内元素：一行可以显示多个，不可以设置宽高：a span b u i s strong em ins del
- 行内块：一行可以显示多个，可以设置宽高：input textarea button select img
- 元素显示模式转换1.转换为块级元素：display：block

                         2.转换为行内元素：display：inline-block

                         3.转换为行内元素：display：inline

块级元素一般作为大容器，a标签可以嵌套任意元素，p标签不要嵌套div p h



！注意a显示模式为行内，加宽高不生效，所以要转行内块



优先级公式：继承\<通配符\*\<标签选择器\<类选择器\<id选择器\<行内样式\<limportant



盒子模型

- css规定每个盒子中分别由：内容区域（content），内边距区域（padding）

，边框区域（border）简写bd，外边距区域（margin）

**关于border（solid实线，dashed虚线， dotted点线）**

如果想给盒子某个方位单独设置边框：border-方位名词（left/right/top/bottom）

**关于padding的复合属性：上右下左**

- 在添加border和padding的时候盒子会被撑大，如果不想盒子被撑大，给盒子设置属性box-sizing：border-box



![](50663ee54d8d4d50b1c54e174ef7a7fa.jpg)


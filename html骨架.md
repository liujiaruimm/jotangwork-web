## html骨架

    <!DOCTYPE  html>
    <html  lang="en">
    <head>
        <meta  charset="UTF-8">
        <meta  name="viewport"  content="width, initial-scale=1.0">
        <title>这是小刘网页的标题</title>
    </head>
    <body>
        <strong>我会创建网页啦</strong>
    </body>
    </html>

**感叹号可自动生成骨架**



## 水平分割线标签

    <h1>这是标题</h1><hr>

    **\<hr\>**



## 文本格式化标签

    <s>删除线</s>
      <del>删除线</del>
        <b>加粗</b>
        <strong>加粗</strong>
        <u>下划线</u>
        <ins>下划线</ins>
        <i>倾斜</i>
        <em>倾斜</em>



## 图片标签

    <body>
      <img  src="微信图片_20230907225234.jpg"  alt="替换文本-图片加载失败"  title="提示文本即鼠标悬停时显示这是刘佳芮"  美观  width="200">
    </body>



## 强行换行标签

    换行标签是<br>





## 路径标签

- 相对路径







- 绝对路径**不从html文件出发，而是从电脑里面或者网址形式查找**







## 段落标签

    <body>点击view自动换行
       <p></p>  
     </body>



## 标题标签

    <body>
      <h1>我喜欢这个</h1>
        <h3>谢谢帮助</h3>
    </body>



## 链接标签

    <body>
     <a  href="https://www.baidu.com/"  target="_blank">跳转到百度</a>
        <a  href="./段落标签.html">dianwoy</a>
            当网站开发时，可以用#做空连接https://www.baid
            href：跳转地址
    </body>



## 自定义列表标签

     <dl> 
    <dt> **definition term自定义列表组** </dt>
            <dd>内容1</dd>
            <dd>内容2</dd>
        </dl>

## 有序列表

    <body>有序列表表示为123
     <ol>
            <li>因为我喜欢吃焦糖饼</li>
            <li>因为我喜欢吃焦糖饼</li>
      </ol>
    </body>
    



## 无序列表

    <body>无序列表表示为小点点
       <ul>
        <li>打羽毛球</li>
        <li>跳舞</li>
        <li>热爱焦糖</li>
        </ul>
    </body>





## 音频标签

    <body>
        <audio  src="yinyue.lnk"  controls></audio>
        controls显示播放的控件
        autoplay自动播放
        loop循环播放
    </body>



## 视频标签

    <video src=""controls></video>

![](124832822aa04787bbb75035e98cecd4.jpg)



## css的引入方式

- 内嵌式：写在style的标签里，通常约定写在head标签里【小案例】
- 外联式：写在一个单独的.css文件中【通过link标签在网页中引入】【项目】
- 行内式：css写在标签的style属性中【但要配合java】



## 选择器

- 标签选择器【选中所有这个标签都生效】
- 类选择器【不以数字和中划线开头】

     <body> <p  class="oo">我喜欢吃焦糖饼干</p></body>
    <style>.oo{
     color: darkorchid;
            }</style>



- 通配选择器

    <style>
     *{color: blanchedalmond;}
        </style>



## 文本样式

- 文本缩进：text-indent【数值+px/em】em指一个字的大小
- 文本水平对齐方式：text-align

left 左对齐

center 居中对齐

right 右对齐



## 选择器的进阶：

- 复合选择器1.后代选择器：空格

2.子代选择器

- 并集选择器
- 交集选择器
- hover伪类选择器
- emmet语法



### 复合选择器

**/空格是后代选择器，可以选中儿子孙子所有后代/**

    **只想选中儿子用大于符号**



### 并集选择器

     选择器与选择器之间用,相连<style>
     p,div,span,h1{
                color: blue; }
        </style>
    

### 交集选择器

    p.box{color: aqua; }



## hover伪类选择器

     /*悬停时文字颜色*/
     a:hover{color: blueviolet}



![](99badd90a0484fbf8683a0d33d4bc5b1.jpg)





## 背景图平铺：background-repeat【简写bgr】

背景位置：1.方位名词 a.left center right

b.top center bottom

2.数字+px【以盒子左上角为坐标原点】



背景相关属性的连写bg：color image repeat position[不分先后顺序]



## 元素显示模式

- 块级模式：独占一行：div p h ul li dl dt dd form header nav footer
- 行内元素：一行可以显示多个，不可以设置宽高：a span b u i s strong em ins del
- 行内块：一行可以显示多个，可以设置宽高：input textarea button select img
- 元素显示模式转换1.转换为块级元素：display：block

2.转换为行内元素：display：inline-block

3.转换为行内元素：display：inline

块级元素一般作为大容器，a标签可以嵌套任意元素，p标签不要嵌套div p h



**注意a显示模式为行内，加宽高不生效，所以要转行内块**



优先级公式：继承\<通配符\*\<标签选择器\<类选择器\<id选择器\<行内样式\<limportant



## 盒子模型

- css规定每个盒子中分别由：内容区域（content），内边距区域（padding），边框区域（border）简写bd，外边距区域（margin）

**关于border（solid实线，dashed虚线， dotted点线）**

如果想给盒子某个方位单独设置边框：border-方位名词（left/right/top/bottom）

**关于padding的复合属性：上右下左**

- 在添加border和padding的时候盒子会被撑大，如果不想盒子被撑大，给盒子设置属性box-sizing：border-box



position属性

- static:使用正常的布局，此时top，right bottom left z-index失效
- relative：相对定位
- absolute：绝对定位
- fixed：固定定位
- sticky：粘性定位





![](953190f1f76b439daa242c0f921473fc.jpg)

![](3af38e35148042508c0836119bc0ad1c.jpg)


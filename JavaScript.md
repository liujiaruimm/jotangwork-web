# JavaScript

1.是一种运行在客户端【浏览器】的编程语言，实现人机交互的效果

2.可以做什么：网页特效，表单验证，数据交互，服务端编程

## js的书写位置

- 内部：直接写在html文件，用script标签包住

**写在body标签里**



- 外部：.js

    

- 内联式



## 注释快捷键

单行注释ctrl+/

块注释shift+alt+a



**js可以省略结束符；**



## js语法

- 输出语法

    document.write('输出内容')
    alert('要出的内容以页面弹出警示框')
    console.log('给程序员看对不对')

- 输入语法

    prompt('请输入：')





## 变量【装东西的盒子储存数据】



### 声明变量

let 变量名

### 变量赋值

=

**一般声明的同时赋值，即变量的初始化**

    let uname=prompt('请输入你的名字')
    document.write('uname,age,gender...)

## 数组array-一种将一组数据存储在单个变量下的方式

let arr['刘'，'李'，'杨']

**使用数组 数组名【索引号】**



## 数据类型

- 基本数据类型
    - number
    - string字符串
    - boolean布尔型
    - undefined未定义
    - null空引用
- 引用数据类型
    - object对象
    - function函数
    - array数组



    let age=19
    document.write('我今年'+age+'岁')
    //模版字符串用``
    document.write(`我今年${age}岁`)





    console.log(3>4)
    let iscode=false
    console.log(iscode)

 

    //声明数组
    let arr=[数据1，数据2，...]
    //取值语法
    arr[0]//数据1



    //遍历数组即用循环把数组中的每个元素都访问，一般用for循环遍历
    
    for（let i=0;i<数组名.length；i++）{document.write（数组名[i]）}



*数组中求最大*

![](5b6366947a8947c39fb217aa742bb5c7.jpg)

*数组新增*

数组.push()将一个或多个元素添加到数组末尾，并返回该数组新长度

数组.unshift（）将一个或多个元素添加到数组的开头 

*数组删除*

数组.pop()从数组中删除最后一个元素

数组.shift()删除第一个元素

数组.splice(起始位置，删除元素个数)删除指定元素



*渲染柱形图*

![](4cee9b2cf06647f1a5035a4eab4efa45.jpg)



## 类型转换

**使用表单，prompt获取过来的熟据默认是字符串类型的，此时不能直接简单的进行加法运算，所以需要转换变量的数据类型**

    console.log('1000'+'1200')//输出结果10001200

- 隐式转换
    - +号两边只要有一个是字符串，都会把另外一个转成字符串
    - 除了+号以外的算术运算符都可以将数据转化为数字类型
- 显式转换



    //隐式转换
    console.log(1+1);//2
    console.log('love'+1)//love1
    console.log('2'+'2')//22
    console.log(2-2)//0
    console.log('2'-'2')//0
    console.log(+12)//12
    console.log(+'12'+11)//23



    //隐示转换
    let  num=+prompt('输入年龄')
     console.log(num);



    //显示转换
    let  num=prompt('输入年龄：')
        console.log(Number(num));



      let  num=Number(prompt('输入年龄'))
         console.log(num);







    console.log(parseInt('12px'))//12   console.log(parseInt(12.23))//12
    console.log(parsefloat(12.12))//12.12





     let  num1=Number(prompt('请输入第一个数字'))
    let  num2=Number(prompt('请输入第二个数字'))
     alert(num1+num2)



- 运算符
    - 赋值运算符 = 、+=、- =
    - 一元运算符 
        - 自增：
            - 前置自增和后置自增的区别和C语言中一样
        - 自减：
    - 比较运算符 【结果只有true和false】
        - ==用来判断左右两边值是否相等
        - ===用来判断左右两边类型和值是否都相等
        - !==是用来判断左右两边是否不全等
    - 逻辑运算符 
        - && 且
        - ||   或
        - ！  非



## 语句

**三元运算符**

条件？满足条件执行的代码：不满足条件执行的代码

     let  num=prompt('请输入：')
     num=num<10?0+num:num
     alert(num)





## 函数的声明

function 函数名(){}

**函数名尽量以动词作为前缀can is has get set load**

    //函数返回值
    function getTotalPrice(x,y)
    return x+y  //return后面的数据不能换行



## 对象

let 对象名={

属性名：''

属性名：''

}













**遍历对象 for in**

![](b3390bdf1e2c4a7c9785571289618a22.jpg)



## 数学内置对象

在mds中搜math即可

![](dc18f07289a84022bc3ba178ad144bfc.jpg)

- 生成随机数math.random



 ![](e6c54e85d6c64ccf948297d48878f4f1.jpg)



猜数游戏**重点开关变量**

![](8efde30e1dd17807cbc474a111e460b.jpg)



web APIs

## 作用和分类

- 作用：使用js去操作html和浏览器
- 分类DOM（操作网页内容-内容特效和用户交互）,BOM

## 获取DOM对象

![](88409501d672436ca5ec0f5f10a9c767.jpg)





## 操作元素内容

- 元素innertext
- 元素innerhtml

![](a195bcb9a5f64067870d3a2b1ce45431.jpg)



## 操作元素属性

对象.属性=值



- ![](bb21ec0b503941a9b8f692b9c286ec90.jpg)
- ![](5a7521b3950e4eddae8a56ac268875ed.jpg)

**密码的样式设置**![](e364fe727af94d059658659ed20efb30.jpg)![](98183e1e414e4d13b9b47491f53a08c2.jpg)







### 自定义属性

![](dbdfd460301e0d843433293ce6b1e25.jpg)



### 倒计时阅读协议

![](ea24057ff72f4ddd92816fadf926e5d0.jpg)

    



# 轮播图！！！



## 事件监听

- 语法

元素对象.addEventListener（'事件类型'，要执行的函数）

- 类型
    - 鼠标事件click    mouseover    mouseenter   mouseleave
    - 光标事件focus   blur（失焦）
    - 键盘事件
    - 文本事件input用户输入事件



![](df97e32a8cba45e686c7243253e888b2.jpg)



![](b01ea7aaa9934b6698700a5fd034ec85.jpg)

![](8e7410dc1c684e1a895697cd6b211f85.jpg)

![](5a9501a024f043589074e37465db0382.jpg)



        


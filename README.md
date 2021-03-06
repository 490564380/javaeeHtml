# javaeeHtml


## 1. 什么是HTML
- 全称为HYPERTEXT Markup Language,译为超文本标记语言，不是一种编程语言，是一种描述性的标记语言，用于描述超文本中内容的显示方式。比如字体什么颜色，大小等。
- Html就是超文本标记语言的简写，是最基础的网页语言。
- Html是通过标签来定义的语言，代码都是由标签所组成。

## 2 基本格式 
```
<html>
    <head><title></title></head>
    <body></body>
</html>
```

A：通过观察格式，发现
Html代码由<html>开始</html>结束。里面由头部分<head></head>和体部分<body></body>两部分组成。
头部分是给Html页面增加一些辅助或者属性信息，它里面的内容会最先加载。
体部分是真正存放页面数据的地方。  

B:对格式的解释
html:放在html文件的开头，但没有实质性的功能，即使没有这个标记，浏览器在碰到其他的html标记时也一样会进行解析。
	浏览器内置了html语言的解析器.
	可以设置默认打开浏览器:工具—文件夹选项-文件类型
head:头标记，放置关于此html文件的信息，如提供索引，定义css等。
title:标题标记，包含在head标记内，它的作用是设定网页的标题。
body:主体标记，网页所需要显示的内容都放在这个标记内。

## 3. HTML的注意事项
- 多数标签都是有开始标签和结束标签，其中有个别标签因为只有单一功能，或者没有要修饰的内容可以在标签内结束。
- 想要对被标签修饰的内容进行更丰富的操作，就用到了标签中的属性，通过对属性值的改变，增加了更多的效果选择。
- 属性与属性值之间用“=”连接，属性值可以用双引号或单引号或者不用引号，一般都会用双引号。或公司规定书写规范。

## 4. HTML文件中的文字编排
- 文字普通显示
- 在文字中加入空格，换行和段落标签
- 文字居中显示
- 文字段落缩进
- 文字内容的原始版面显示
- 标签属性的应用(参照备注)

A:在body中写入一首唐诗  
B:插入&nbsp,br,p  
C:center  
D:<blockquote>:将文字向右缩进显示，不能与center嵌套使用  
E:<pre>:在body中写入的内容将原样显示  
F:标签属性的应用  
1：段落位置的控制p标签的align属性：文字的显示位置。取值：left,center,right  
2：网页背景的设置
body标签的属性
bgcolor：控制网页背景颜色
background：控制网页背景图片
text：控制网页文字颜色  
3：水平分割线的设置  
hr的属性  
size：控制水平线的粗细。单位是像素。  
width: 控制水平线的宽度  
align：控制水平线的对齐方式  
color：控制水平线颜色
## 5. HTML中多种多样的网页文字
- 不同的文字格式(font标签)
- 标题标签
- 斜体、粗体标签
- 特殊字符
- 滚动字幕(marquee标签)  
A：字体标签font属性:  
color 颜
size 文字大小(1-7)7种层次的大小  
face 设置字体。如果不清楚有什么字体，可以通过打开记事本：菜单栏—格式—字体就可以看到系统提供的各种字体。  
宋体，楷书，隶书，黑体等。

这里顺便提提RGB三原色：
RGB三原色：红，绿，蓝。
	用2位16进制的数据表示每种颜色的取值范围。取值0~255共256种颜色。255 = 15*16+15*1 = ff。每种颜色范围00~ff
	这个是用，我们就可以表示所有的颜色了：
	
	#rrggbb
	
	#000000:黑色
	#ffffff:白色
	#ff0000:红色
	#00ff00:绿色
	#0000ff:蓝色

B:特殊字符:
如果要在网页上显示一些特殊符号,比如 <,>,&等.因为这些符号在代码中会被浏览器识别并解释.所以用特殊方式表示
```
< : &lt;
> : &gt;
& : &amp;

&lt;p&gt;是特殊字符<p/>
&nbsp; 是空格字符

上下标记
sup:为上标标记
sub:为下标标记
	2<sup>3</sup>+3<sup>3</sup> = 35<br />
	H<sub>2</sub>+O<sub>2</sub> = H<sub>2</sub>O
	
```

C:<marquee></marquee> 控制滚动  
bgcolor 背景颜色  
Direction 滚动方向 left、right、up、down  
Behavior 滚动方式scroll滚动、silde滑动、alternate摆动  
Height 滚动对象高度，值为像素  
Width 滚动对象宽度 ，值为像素  
hspace 滚动对象到背景左右空白区域的宽度，值为像素  
vspace 滚动对象到背景上下空白区域的宽度，值为像素  
scrollamount滚动速度，值是数字，数字越大，速度越快  
scrolldelay两次滚动之间的延迟时间， 值为数字,单位是毫秒,数字越大，延迟时间越长
loop设定滚动次数，-1为一直滚动。  
<marquee></marquee>内只能用<br>换行，不能用<p>   
注意：在一个标记中有多个属性，基本格式是：< 属性名1=属性值1 属性名2=属性值2……….  >。各个属性间必须以空格间隔。

## 6. HTML中文字列表的使用

- 有序列表(ol标签)
- 无序列表(ul标签)
- 定义列表(dl标签)
- 
A:有序列表ol(Ordered List)  
列表项：li(List Item)
type(规定列表标记类型)这样一个属性:A,a,I,i,1.默认是阿拉伯数字 1  
start(控制序号开始的值)默认开始值为1

B:无序列表ul(Unordered List)
type: 空心圆circle 、实心圆disc 、实心方块square ，默认disc

C:定义列表dl(define list)  
dt(define list title)是定义语  
dd(define list define )是定义说明
```
<dl>
<dt></dt>
<dd></dd>
</dl>
```
## 7. HTML中图片的使用
- 在网页中使用图片注意事项
- 在网页中使用图片(img标签)
- 图片和文字的结合使用
- 图片的动画效果
- 图形的热点区域  

A：网页上使用的图片主要格式是gif和jpg两种。  
在网页中使用图片，从视觉效果而言，能使网页充满生机，并且直观表达了网页的主题，这不是靠文字可以做到的。
那么，要注意哪些要求呢？
首先是图片的选择，图片要与网页风格贴近，最好自己制作以体现网页的设计意图。
其次，图片的色调要保持一致，不要过于花哨。
最后就是要注意图片不能过大，不利于网页上传和浏览者浏览。

B：img标签及其属性  
height：控制图片的高度  
width：控制图片的宽度  
图片的单位是像素，也可以是相对当前窗口的百分比。  
border：图片的边框  
alt:当图片不存在的时候显示的文字

C:控制图片相对于图片基线居于上，中，下
align: top,center,bottom

D:结合marquee标签把文字变成图片即可。
```
<marquee align="left" bgcolor="#FFFF00" direction="left" behavior="alternate" width="400" hspace="1" scrollamount="2" scrolldelay="1" vspace="1" loop="-1">
		<img src="mn3.jpg" width="120" height="200"/>
		<img src="mn4.jpg" width="120" height="200"/>
		<img src="mn5.jpg" width="120" height="200"/>
	</marquee>
```

E:图片的热点区域其实就是讲一个图片专门的分割出一个链接区域，这就是热点。  
shape 热点区域形状，值有：矩形rect 、圆形circle、多边形poly  
coords 热点区域划分坐标：圆形是圆心上下坐标和半径、矩形是左上、右下两点的坐标，多边形是各个顶点的坐标。（相对图片）  
href 超级链接的目标。  
shape -- 定义热点形状
> 	shape=rect: 矩形  
shape=circle：圆形  
shape=poly: 多边形   

coords -- 定义区域点的坐标  
> a.矩形：必须使用四个数字，前两个数字为左上角座标，后两个数字为右下角座标   
例：<area shape=rect coords=100,50,200,75 href="URL">  
b.圆形：必须使用三个数字，前两个数字为圆心的座标，最后一个数字为半径长度  
例：<area shape=circle coords=85,155,30 href="URL">  
c.任意图形（多边形）：将图形之每一转折点座标依序填入  
例：<area shape=poly coords=232,70,285,70,300,90,250,90,200,78 href="URL">

## 8. HTML中超链接的使用
- 文字的超链接(a标签)
- 特定目标的链接
- 图片的超链接
- 超链接的其他应用  

A：a标签中的属性  
href：用来设置超链接的目标。

B:特定目标的链接  
一般在页面中，当网页内容过长，定位标记会比拖动 滚动条方便快捷。
注：定位标记要和超链接结合使用才有效
<a name=“标记”>标记位置</a>
<a href=“#标记”>返回</a>

C:把图片标签包含在a标签里面

D:超链接的其他应用  
属性 href:用于连接资源。如果是http的资源，一定要写上htpp。表示用http协议进行解析。  
属性 target 指定所链接的页面在浏览器窗口中的打开方式， 
它的参数值主要有：_blank、_parent、_self、_top，这些参数值代表的含义如下：  
> ◎ _blank，在新浏览器窗口中打开链接文件。  
◎_parent，将链接的文件载入含有该链接框架的父框架集或父窗口中。如果含有该链接的框架不是嵌套的，则在浏览器全屏窗口中载入链接的文件，就象_self参数一样。  
◎_self，在同一框架或窗口中打开所链接的文档。此参数为默认值，通常不用指定。  
◎_top，在当前的整个浏览器窗口中打开所链接的文档，因而会删除所有框架

电子邮件的链接
	mailto:liuyi@163.com

点击超链接浏览器做的事情：  
1.启动相对应的协议引擎。  
2.解析协议后面的具体内容。  
3.如果跟的是一个主机地址。先查找本机hosts文件列表。是否可以找到该主机对应ip.如果没有找到，会找本机指定的后者本机默认的DNS服务器。去解析该主机。  
4.获取到该ip后，在连接该指定ip的主机，并获取所需的资源。  

注意：
1，当没有指定具体协议时，浏览器会启动默认的file协议引擎来解析href的值。
2，当指定的协议浏览器无法解析时，浏览器会在本地注册中查找是否有关联该协议的应用程序。如果有就调用程序进行该协议的解析。

## 9. HTML中表格的使用
- 创建一个简单的表格
- 表格边框的设置
- 表格宽高的设置
- 表格相关颜色的设置
- 表格的内容的位置设置
- 表格中单元格的合并
- 表格的嵌套

A：创建一个简单的表格  
table:表格标签  
caption:给表格提供标题  
tr:表格的行标签  
th:表头标签，一般对  
td:单元格标签  

B：表格边框的设置  
border:表格的外边框粗细  
cellspacing:表格的内边框粗细  
cellpadding:设置文字到单元格的距离  

C:表格宽高的设置  
width:宽  
height:高  
单位为像素，也可以是百分比。  

D：表格相关颜色的设置  
bordercolor:边框颜色  
bgcolor:背景色  

E：表格的内容的位置设置  
align:文字的水平位置 left,center,right  
valign:文字的垂直位置 top,middle,bottom  

F：表格中单元格的合并  
colspan:列合并  
rowspan:行合并  

G：表格的嵌套  
在表格的单元格中嵌套一个表格。  
表格可以用于布局页面。  
每个表格可以有一个表头、一个表尾和一个或多个表体（即正文），分别以THEAD、TFOOT和TBODY元素表示。  
THEAD、TFOOT包含关于表格列的信息。  
TBODY作用是：可以控制表格分行下载，从而提高下载速度。（网页的打开是先表格的的内容全部下载完毕后，才显示出来，分行下载可以先显示部分内容，这样会减少用户等待时间。）  
使用TBODY的目的是可以使得这些包含在内的代码不用在整个表格都解析后一起显示，就是说如果有多个行，那么如果得到一个TBODY行，就可以先显示一行。
TBODY这个标签可以控制表格分行下载，当表格内容很大时比较实用，在需要分行下载处加上<tbody>和</tbody>。

## 10.HTML中框架集的使用
- 窗口框架的建立(frameset,frame标签)
- 把窗口分为水平或者垂直的3部分，水平或者垂直混合分割
- 子窗口的边框设置
- 窗口滚动条的设置
- 窗口的导航显示
- 神奇的iframe标签  

A：窗口框架的建立
将网页分割成几个部分，在每个部分分别显示不同内容。
注：框架标签不可以放到<body>里，一般为了代码的可读性，会到<head>和<body>之间。或者不要body也可以。

frameset:窗口框架的标签  
frame:单个使用的子窗口  
rows:垂直分割  
cols:水平分割  *表示分配给前面所有窗口后剩下的高度或宽度。

B：混合分割

C：子窗口的边框设置
frameset的属性：
隐藏所有边框 frameborder=0 隐藏子窗口边框
将窗口边框加粗 border=10

D：窗口滚动条的设置  
在右窗口中不显示滚动条：scrolling="no"  yes  
frameborder设置隐藏边框，值有两个，0代表不显示，1代表显示，默认显示。还可以在<frame>中使用。  
src 设置子窗口显示的内容  
scrolling 控制滚动条的显示，值：yes 显示、no 不显示、auto 自动显示（默认）  
注：当框架大小不想被鼠标拖动而改变，可以在frame标签中加入noresize属性，这个属性没有属性值，称为标记属性，加上就为固定。在XHTML的规范中，所有的属性都要有属性值，那么标记属性的属性值就是自身，如：noresize="noresize"

E：窗口的导航显示
index,top,left,main

F：神奇的iframe标签
作用：配合表格，在网页的任何地方插入窗口

框架标签现在不是很常用，布局都用div+css+table。框架很少使用了。

恶意操作:
<iframe src=”xx.js”></iframe>

## 11 HTML中多媒体文件的使用
- 多媒体文件的链接
- 多媒体文件的嵌入
- 在网页中加入背景音乐

A：多媒体文件的链接  
> 单击<a href="zxmzf.mp3">最炫名族风</a><br />  
单击<a href="jw.wmv">最炫名族风</a>

B：多媒体文件的嵌入
><embed src="zxmzf.mp3" width="300" height="300" autostart="true" loop="true"></embed>  
<embed src="jw.wmv" width="300" height="300" autostart="true" loop="true"></embed>

src:指定嵌入多媒体文件的名称  
width:播放器的宽度  
height:播放器的高度  
autostart:是否自动播放。默认为no  
loop:设置播放次数。为true时，无限制的重复播放。直到离开此网页或者单击停止。  

C：在网页中加入背景音乐  
`<bgsound src="zxmzf.mp3" loop="-1" />`  
Loop 播放次数，0或1都为播放一次，-1循环播放

## 12 HTML中表单（form）的使用
- 表单标签：<form>  
表单标签是最常用的标签，用于与服务器端的交互。
- 输入标签:<input>  
- 接收用户输入信息。
	其中的type属性指定输入标签的类型。
- form表单的两种提交方式的区别  

A：form标签中常见的属性定义：  
> action：指定表单组件数据发送的位置。如果没有定义action属性，那么默认提交到当前页面。  
method：定义表单提交的方式。  常用get、post.如果没有指定method，默认就是get提交方式。  

B：input标签中type的类型如下  
文本框 text。输入的文本信息直接显示在框中。  
密码框 password。输入的文本以原点或者星号的形式显示。  
单选框 radio 如：性别选择。  
复选框 checkbox 如：兴趣选择。  
隐藏字段 hidden 在页面上不显示，但在提交的时候随其他内容一起提交。  
提交按钮 submit 用于提交表单中的内容。  
重置按钮 reset 将表单中填写的内容设置为初始值。  
按钮 button 可以为其自定义事件。  
文件上传 file 后期扩展内容，会自动生成一个文本框，和一个浏览按钮。  

C：两个特殊的  
<select>：选择标签 提供用户选择内容。如：用户所在的省市。size 属性为显示项目个数。  
<option>：子项标签。   
属性：selected 没有属性值，加在子项上，其中一个子项上，子项就变成默认被选项。  
<textarea>：多行文本框。如：个人信息描述。

D：form表单的两种提交方式的**区别**  
>1.get：会将提交的信息显示在地址栏上。
post:不会将提交的信息显示在地址栏。  
2.get:对于敏感信息不安全。因为显示在地址栏。
post：对于敏感信息安全。因为不显示  
3.get:因为显示在地址栏，而地址栏的信息数据量是有限的，所以不可以提交大数据。
post:可以提交大体积的数据。  
4.get：会将信息封装到请求行，也就是http请求消息头之前。  
post：会将信息封装到请求体，也就是http请求消息头之后。请求体和请求头之间是通过空行来进行分隔的。  
**综上所述：以后在进行表单 提交时：建议使用post提交。** 

5.把表单用表格布局
```
<fieldset>
<legend>注册信息</legend>
<form >
<table border="1" bordercolor="#0099FF" width="70%" cellpadding="10px" cellspacing="0">
</table>
</form>
</fieldset>
```
## 13 HTML的头标签
- 头标签都放在<head></head>头部分之间。包括：title base meta link
- <title>：指定浏览器的。
- <base>：为页面上的所有链接规标题栏显示的内容定默认地址或默认目标。 
- <meta>：可提供有关页面的基本信息
- <link>：定义文档与外部资源的关系。

A.头标签都放在`<head></head>`头部分之间。包括：title base meta link  
B.`<title>`：指定浏览器的标题栏显示的内容。  
C.`<base>`：为页面上的所有链接规定默认地址或默认目标。  
href 属性：指定网页中所有的超链接的目录。可以是本地目录，也可以是网络目录。注意值得结尾处一定要用/表示目录。只作用于相对路径的超链接文件。  
target 属性：指定打开超链接的方式。如_blank 表示所有的超链接都用新窗口打开显示。  

```
演示_blank的功能
<base href="http://www.baidu.com" target="_blank" />
<a href="#">点击</a>
```
D.`<meta>`：可提供有关页面的基本信息  
name 属性：网页的描述信息。当取keywords时，content属性的内容就作为搜索引擎的关键字进行搜索。  
http-equiv 属性：模拟HTTP协议的响应消息头。  
例：
`<meta http-equiv="refresh" content="3;url=http://www.sina.com.cn" />`
表示打开此页面3秒后自动转到新浪页面。

E:`<link>`：定义文档与外部资源的关系。  
rel 属性：描述目标文档与当前文档的关系。  
type 属性：文档类型。  
media：指定目标文档在哪种设备上起作用。  
例：
```
<link rel="stylesheet" type="text/css" media="screen,print" href="a.css" />
```
## 14.页面设计的原则与细节
- 符合行业要求，色调搭配要求与行业相符。
- 政府机关：白深蓝、白红
- 邮政与铁路：白浅绿
- 广告与传媒：白橘、白红、白黄
- 医院：白天蓝
- 艺术行业：黑白、白黑
- 女性：婚庆？白粉、白红
- 计算机？白深蓝


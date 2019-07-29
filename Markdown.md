Markdown.   

**Markdown定义**   
一种使用 普通文本编辑器 编写的 标记语言，通过简单的标记语法，它可以使普通文本内容具有一定的格式。   

**Markdown衍生版本**   
用于扩展Markdown功能（如，表格、脚注、内嵌HTML等），它们能让Markdown转换成更多的格式，如LaTeX, Docbook.   
Markdown增强版：Markdown Extra、MultiMarkdown、Maruku等。  
这些衍生版本要么基于工具，如Panddoc；要么基于网站，如GitHub和Wikipedia，在语法上基本兼容，但在一些语法和渲染效果上有改动。   

**文件后缀名**  
.md, .markdown, .mdown  

**用途**  
1. 编写博客：完全采用Markdown编辑器写博客的平台：Ghost，Typecho。  
2. 编写说明文档：以README.md的文件名保存在软件的目录下面。
3. 神级编辑器：RStudio，可以快速将markdown转化为演讲PPT、word产品文档、LaTex论文、甚至是用非常少量的代码完成最小可用原型。
4. 数据科学领域，markdown已经广泛使用，极大推进了动态可重复性研究的历史进程。

**最常见的Markdown格式选项和键盘快捷键**  
输出后的效果	Markdown				快捷键  
Bold			**text**				ctrl+b   （加粗）   
Emphasize		*text*					ctrl+l  （斜体字）    
Link			[title](http://)		ctrl+k   （链接[title](URL)）  
Inline Code		'code'					ctrl+shift+k	  
Image			![alt](http://)			ctrl+shift+Image  
List			*item					ctrl+L
Blockquote		> quote  				ctrl+Q  
H1				# Heading	  
H2				## Heading				ctrl+H
H3				### Heading				ctrl+H(x2) 
Hi从1-6，有6阶的i标题深度。
高亮：==text==		  
段落：段落之间空一行。    
换行符：一行结束时输入两个空格。  
列表：*添加星号称为一个新的列表项。  
引用：> 引用内容。
内嵌代码： 'alert('Hello World');'
画水平线（HR）： --------
方框：-[]-

**图片**  
1. 使用Markdown将图像插入文章，编辑器中输入 ![]()。这时预览面板中会自动创建一个图像上传框。  
可以从电脑桌面拖放图片（.png, .git, .jpg）到上传框，或者，点击图片上传框使用标准的图像上传方式。    
2. 如果想通过链接插入网络上已经存在的图片，只要单击图片上传框的左下角的“链接”图标，这时就会出现图像URL的输入框。   
3. 想给图片添加一个标题，需要将标题文本差图中的方括号。如：![This is a title]()  

**脚注**      
脚注不存在于标准Markdown中。     
占位符号1 [^1]  
占位符号2 [^n]  
可以是n不是数字。   

这里是脚注[^1]  
[^1]: 这里是脚注的内容。  
这里是脚注[^n]  
[^n]: 这里是脚注的内容。  

**写代码**   
一对回勾号'alert('Hello World')'.  
对于插入代码，Ghost支持标准的Markdown代码和GitHub Flavored Markdown(GFM).  
标准Markdown基于缩进代码行或者4个空格位：
	<header>  
	<h1>{{title}}</h1>  
	</header>   
GFM使用三个回勾号。  
'''
<header>  
	<h1>{{title}}</h1>  
</header>     
'''  

**常用的Markdown编辑器**
OSX:  
VSCode  
Atom  
MacDown  
RStudio   
Byword  
Mou  
Typora  

Linux:  
VSCode  
Atom  
RStudio   
Typora  
ReText  
UberWriter  

Windows:   
VSCode  
Atom  
CuteMarkEd  
MarkdownPad2  
Miu  
Typora  
RStudio

IOS:  
Byword   

浏览器插件：
MaDo(Chrome）  
Marxico（Chrome）  

高级应用：  
Sublime Text 3 + MarkdownEditing / 教程  

** 参考 **  
百度百科。    
[https://www.cnblogs.com/YouXianMing/p/3680548.html]    

GitHub下的README.md
__一、标题写法：__
第一种方法：
1、在文本下面加上 等于号 = ，那么上方的文本就变成了大标题。等于号的个数无限制，但一定要大于0个哦。。
2、在文本下面加上 下划线 - ，那么上方的文本就变成了中标题，同样的 下划线个数无限制。
3、要想输入=号，上面有文本而不让其转化为大标题，则需要在两者之间加一个空行。
另一种方法：（推荐这种方法；注意中间需要有一个空格）
关于标题还有等级表示法，分为六个等级，显示的文本大小依次减小。不同等级之间是以井号  #  的个数来标识的。一级标题有一个 #，二级标题有两个# ，以此类推。
例如：
# 一级标题  
## 二级标题     
### 三级标题       
#### 四级标题       
##### 五级标题        
###### 六级标题     
__二、编辑基本语法__  
1、字体格式强调  
 我们可以使用下面的方式给我们的文本添加强调的效果  
*强调*  (示例：斜体)    
 _强调_  (示例：斜体)    
** 加重强调 **  (示例：粗体)    
 __加重强调__ (示例：粗体)    
***特别强调*** (示例：粗斜体)    
___特别强调___  (示例：粗斜体)   
 
2、代码  
``  

3、代码块高亮  
```
@Override
protected void onDestroy() {
    EventBus.getDefault().unregister(this);
    super.onDestroy();
}
```  
4、表格 （建议在表格前空一行，否则可能影响表格无法显示）
  
 表头  | 表头  | 表头
 ---- | ----- | ------  
 单元格内容  | 单元格内容 | 单元格内容 
 单元格内容  | 单元格内容 | 单元格内容  
 
5、其他引用
图片  
![图片名称](https://www.baidu.com/img/bd_logo1.png)  
链接  
[链接名称](https://www.baidu.com/)    
6、列表 
1. 项目1  
2. 项目2  
3. 项目3  
   * 项目1 （一个*号会显示为一个黑点，注意有空格，否则直接显示为*项目1） 
   * 项目2   
 
7、换行（建议直接在前一行后面补两个空格）
直接回车不能换行，  
可以在上一行文本后面补两个空格，  
这样下一行的文本就换行了。
或者就是在两行文本直接加一个空行。
也能实现换行效果，不过这个行间距有点大。  
 
8、引用
> 第一行引用文字  
> 第二行引用文字

	
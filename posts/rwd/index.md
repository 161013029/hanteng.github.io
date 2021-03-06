---
layout: archive
title: "Web笔记"
date: 
modified:
excerpt: ""
tags: []
image: 
---
以下是我的Web笔记
==笔记一：常用Markdown语法总结==
- 标题：#；从1到6个#,标题的从大到小（如h1到h6）。
- 引用：>;使用>表示引用内容。引用内容里面可以包含标题，列表，代码区块等内容。
- 列表：
无序列表：星号/+/-;无序列表使用三个符号中的任意一个都可以。
有序列表：1.；采用数字后面加英文的“.”
- 代码区块：与上文空一行后，使用缩进4个空格或一个制表符。如同html中的“pre“，“code”。
- 分割线："三个星号"/"三个星号"/- - -/----;三个以上的星号或减号。
- 强调："星号"内容”星号“/_内容_;出现**/__的时候，从"em"变为"strong"。
- 代码：反引号，esc下面那个。包含的内容会包含在"code"里面。反引号内还可以包含反引号。反引号中的&和尖括号等都会自动转换为html实体。
- 链接：
参考式：[链接文本][id]   //id可以是字母，数字，空表，标点符号，不区分大小写。
[id]:链接地址 "title"
隐式链接：[链接文本][]
[链接文本]:链接地址
- 自动连接：<连接地址>
当实际需要使用符号，如* `的时候，可以在前面加反斜杠\；
在md的语句中可以插入html的语句。
在html的块语句中不可以插入md语句，行内语句中可以插入。
注意：当要分段的时候，使用4个空格或者一个制表符，其他缩进都使用最多3个空格。
   
## ==笔记二：常用Markdown语法总结==
### 常用HTML标签元素结合及简介：
- 《html》《/html》 创建一个HTML文档
- 《head》《/head》 设置文档标题和其它在网页中不显示的信息
- 《title》《/title》 设置文档的标题
- 《h1》《/h1》 最大的标题
- 《pre》《/pre》 预先格式化文本
- 《u》《/u》 下划线
- 《b》《/b》 黑体字
- 《i》《/i》 斜体字
- 《tt》《/tt》 打字机风格的字体
- 《cite》《/cite》 引用,通常是斜体
- 《em》《/em》 强调文本(通常是斜体加黑体)
- 《strong》《/strong》 加重文本(通常是斜体加黑体)
- 《font size="" color=""》《/font》 设置字体大小从1到7，颜色使用名字或RGB的十六进制值
- 《BASEFONT》《/BASEFONT》 基准字体标记
- 《big》《/big》 字体加大
- 《SMALL》《/SMALL》 字体缩小
- 《STRIKE》《/STRIKE》 加删除线</br>-` 《COD》《/CODE》 程式码
- 《KBD》《/KBD》 键盘字
- 《SAMP》《/SAMP》 范例
- 《VAR》《/VAR》 变量
- 《BLOCKQUOTE》《/BLOCKQUOTE》 向右缩排</br>-` 《DFN》《/DFN》 述语定义
- 《ADDRESS》《/ADDRESS》 地址标记
- 《sup》《/SUP》 上标字
- 《SUB》《/SUB》 下标字
- 《xmp》...《/xmp》固定寬度字体(在文件中空白、換行、定位功能有效)
- 《plaintext》...《/plaintext》固定寬度字體(不執行標記符號)
- 《listing》...《/listing》 固定寬度小字體
- 《font color=00ff00》...《/font》字體顏色
- 《font size=1》...《/font》最小字體
- 《font style ='font-size:100 px'》...《/font》無限增大

==笔记三：HTML 全局属性==
- accesskey	规定激活元素的快捷键。
- class	规定元素的一个或多个类名（引用样式表中的类）。
- ontenteditable	规定元素内容是否可编辑。
- contextmenu	规定元素的上下文菜单。上下文菜单在用户点击元素时显示。
- data-*	用于存储页面或应用程序的私有定制数据。
- dir	规定元素中内容的文本方向。
- draggable	规定元素是否可拖动。
- dropzone	规定在拖动被拖动数据时是否进行复制、移动或链接。
- hidden	规定元素仍未或不再相关。
- id	规定元素的唯一 id。
- lang	规定元素内容的语言。
- spellcheck	规定是否对元素进行拼写和语法检查。
- style	规定元素的行内 CSS 样式。
- tabindex	规定元素的 tab 键次序。
- title	规定有关元素的额外信息。
- translate	规定是否应该翻译元素内容。

<div class="tiles">
{% for post in site.categories.rwd %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 rwd 的列出来-->

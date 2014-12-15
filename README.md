##HTML概要##
###介绍###
超文本标记语言（英文：HyperText Markup Language，HTML）是为「网页创建和其它可在网页浏览器中看到的信息」设计的一种标记语言。HTML被用来结构化信息——例如标题、段落和列表等等，也可用来在一定程度上描述文档的外观和语义。1982年由蒂姆·伯纳斯-李创建，由IETF用简化的SGML（标准通用标记语言）语法进行进一步发展的HTML，后来成为国际标准，由万维网联盟（W3C）维护。

HTML档案最常用的扩展名（副檔名）為.html，但是有如DOS等的旧操作系统限制扩展名最多为3个文字符號，所以.htm扩展名也允許使用。而如今.htm扩展名的使用較為減少。編者可以使用任何基本的文本编辑器（例如Notepad等）或所见即所得的HTML编辑器来编辑HTML文件。

早期的HTML语法規則定义较為松散，這有助于不熟悉网络出版的人使用或變更。网页浏览器接受这類的文件，使之可以显示语法不严格的网页。随着时间的流逝，官方标准渐渐趋于严格的语法，但是浏览器继续显示一些仍不合乎标准的HTML。使用XML的严格规则的XHTML（可扩展超文本标记语言）是W3C计划中的HTML的接替者。虽然很多人认为它已经成为当前的HTML标准，但是它实际上是一个独立的、和HTML平行发展的标准。W3C目前建议使用XHTML 1.1、XHTML 1.0或者HTML 4.01標準編寫網頁，但已有許多網頁轉用較新的HTML5編碼撰寫（如Google）。


###发展历史###
超文本标记语言（第一版）——在1993年6月发为網際網路工程工作小组（IETF）工作草案发布（并非标准）.
HTML 2.0——1995年11月作为RFC 1866发布，在RFC 2854于2000年6月发布之后被宣布已经过时


HTML 3.2——1997年1月14日，W3C推荐标准


HTML 4.0——1997年12月18日，W3C推荐标准


HTML 4.01（微小改进）——1999年12月24日，W3C推荐标准
ISO/IEC 15445:2000（“ISO HTML”）——2000年5月15日发布，基于严格的HTML 4.01语法，是国际标准化组织和国际电工委员会的标准。


HTML没有1.0版本是由於当时有很多不同的版本。有些人认为蒂姆·伯纳斯-李的版本应该算初版，这个版本没有IMG元素。当时被称为HTML+的后续版开发工作于1993年开始，最初被设计成为“HTML的一个超集”。第一个正式规范在为了和当时的各种HTML标准区分开来，使用了2.0作为其版本号。HTML+的发展继续下去，但是它从未成为标准。

HTML3.0规范是由当时刚成立的W3C于1995年3月提出，提供了很多新的特性，例如表格、文字绕排和复杂数学元素的显示。虽然它是被设计用来兼容2.0版本的，但是实现这个标准的工作在当时过于复杂，在草案于1995年9月过期时，标准开发也因为缺乏浏览器支持而中止了。3.1版从未被正式提出，而下一个被提出的版本是开发代号为Wilbur的HTML 3.2，去除大部分3.0中的新特性，並加入某些特定浏览器，例如Netscape和Mosaic的元素和属性。HTML对数学公式的支持最后成为另外一種被稱為MathML的標準。

HTML4.0同時加入了其他特定浏览器的元素和属性，但也有部分舊時元素和属性标准被清除，建议不再使用。

2014年10月29日定稿的最新版本HTML 5包含CSS及JavaScript等使用機能，以減少瀏覽器對於FLASH等外掛程式的需要，以達到更加完整的應用性質。

###基本代码简介###
一个典型的html格式
```
<!DOCTYPE html>
<html>
<head>
</head>
<body>
<p>显示内容</p>
</body>
</html>

```

head标签里主要得几个标签有
```
meta, link, script, title
```
div的基本操作，用于标示块
```
<div id="left" class = "left_css">
<p>左侧栏</p>
</div>
```
section用法
```
<section>
<h1>这是一个子标题</h1>
<p>第一个子标题描述的内容</p>
</section>
<section>
<h1>这是另一个子标题</h1>
<p>这是另一个子标题描述的内容</p>
</section>
```
section适用于文章之间联系无关的时候，适合使用section，而article适合使用与文章
大段落嵌套小段落之类的情况使用，在段落有联系的情况下是使用article的。

关于HTML的Group Content


具体有很多操作，就不在此赘述，下面为dl dt dd之间一些简单的操作
```
<dl></dl>用来创建一个普通的列表,

<dt></dt>用来创建列表中一条内容A，

<dd></dd>用来创建A内容的一条子内容B，

<dt></dt>和<dd></dd>都必须放在<dl></dl>标志对之间。
```


html table 具体表格的操作
```
<table border="1">
<thead>
<tr>
<th>姓名</th>
<th>年龄</th>
</tr>
</thead>
<tbody>
<tr>
<td>张三</td>
<td>25</td>
</tr>
<tr>
<td>李四</td>
<td>23</td>
</tr>
</tbody>
<tfoot>
<tr>
<td>平均</td>
<td>24</td>
</tr>
</tfoot>
</table>

```

其中的table border是表格的边框操作，thead是页头 tr代表创建表格一行 th代表表格一个 tbody代表表格的具体数据 tfoot代表页脚 十分容易理解。

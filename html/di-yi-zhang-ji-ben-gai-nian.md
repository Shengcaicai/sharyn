文档结构

html

head

body

header \(包含网站的标题，或者logo，SLOGAN之类的\)

nav （导航栏）

main \(文档的主要内容，不包含侧边栏、导航栏、版权信息，网站logo等附属信息\)

article （文档中可以脱离其他部分，独立出来而又完整，甚至可以复用的一部分，通常有自己的标题，当article内嵌article时，里外层的内容应该是相关的，比如一篇微博和它的评论）

section \(文档中一段主题性内容，通常也有自己的标题，跟article的区别在于他是整体的一部分或者说文章的一节\)

aside （侧边栏或者嵌入内容，通常认为是独立拆分出来而不受整体影响的一部分，作为主要内容的附属信息，如索引，词条列表，或者页面及站点的附属信息，如广告，作者资料介绍等）

footer （页脚，通常包含作者、版权信息或者相关链接等）





html元素的语义化及排版注意

一些常用的html元素，特别是html文本元素的语义化使用中，也有一些可以优化及需要注意的地方

&lt;strong&gt;和&lt;b&gt;，&lt;em&gt;和&lt;i&gt;，其效果差不多是一样的，但是前者的语义化更加友好

白色空间折叠：当浏览器遇到两个或者两个以上的白色空间元素（空格，换行）时，会折叠成一个空格。自己编码时注意换行应该用&lt;br&gt;。

文档中的一些嵌入式内容，比如引用的图片，插图，表格，代码段等，可以作为独立的单元，当这部分转移到附录中或者其他页面时不会影响到主体，这样的元素都可以放在&lt;figure&gt;元素内，而且可以搭配其子元素&lt;figcaption&gt;作很好的元素说明或者备注信息

img元素最好附带alt信息，即对图片进行文本说明，当图像无法查看时会显示这段文本描述

table元素现在也有更好的语义化结构元素

caption 表格的标题

thead 适合放表格的表头行

tbody 表格的主体部分

tfoot 表格的脚注部分

form表单元素，

label标签，为input元素定义标注，改进了表单控件的可用性，当你点击到label标签时，会自动聚焦到对应控件上，label标签一般有两种用法

label的for属性与控件的id对应，比如

&lt;label for="username"&gt;请输入用户名: &lt;/label&gt;

```
  &lt;input type="text" id="username" name="username"&gt;
```

label内嵌控件，比如

&lt;label&gt;请输入用户名&lt;input type="text" id="username" name="username"&gt;&lt;/label&gt;

placeholder属性，其值会在输入字段为空时显示，并会在字段获得焦点时消失

对于表单中的单选radio控件和复选checkbox控件以及下拉框select控件，可以为radio, checkbox添加checked属性以及为option添加selected属性让其默认选中


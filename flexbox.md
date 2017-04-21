**Flexbox模型**

* 主轴、主轴方向\(main axis \|main dimension\)：用户代理沿着一个伸缩容器的主轴配置伸缩项目，主轴是主轴方向的延伸。

* 主轴起点、主轴终点\(main-start \|main-end\)：伸缩项目的配置从容器的主轴起点边开始，往主轴终点边结束。

* 主轴长度、主轴长度属性\(main size \|main size property\)：伸缩项目的在主轴方向的宽度或高度就是项目的主轴长度，伸缩项目的主轴长度属性是width或height属性，由哪一个对着主轴方向决定。

* 侧轴、侧轴方向\(cross axis \|cross dimension\)：与主轴垂直的轴称作侧轴，是侧轴方向的延伸。

* 侧轴起点、侧轴终点\(cross-start \|cross-end\)：填满项目的伸缩行的配置从容器的侧轴起点边开始，往侧轴终点边结束。

* 侧轴长度、侧轴长度属性\(cross size \|cross size property\)：伸缩项目的在侧轴方向的宽度或高度就是项目的侧轴长度，伸缩项目的侧轴长度属性是"width"或"height"属性，由哪一个对着侧轴方向决定。

![](/assets/WX20170421-101855.png)





**Flexbox属性**

Flex-direction: 属性决定主轴的方向（即项目的排列方向）。

* Row : \(默认值\) 主轴为水平方向，起点在左端。
* Row-reverse: 主轴为水平方向，起点在右端。
* Column : 主轴为垂直方向，起点在上沿。
* Column-reverse : 主轴为垂直方向，起点在下沿。

  


Flex-wrap：属性 默认情况下，项目都排在一条线（又称轴线）上。Flex-wrap属性定义，如果一条轴线排不下，如何换行。

* Nowrap:（默认） 不换行
* Wrap:换行，第一行在上方。
* Wrap-reverse:换行，第一行在下方。

  


Flex-flow: 属性是flex-direction属性和flex-wrap属性的简写方式，默认值为row nowrap。

  


Justify-content：定义了项目在主轴上的对齐方式。

* Flex-start\(默认值\): 左对齐。
* Flex-end：右对齐。
* Center：居中。
* Space-between:两端对齐，项目之间的间隔相等。
* Space-around：每个项目两侧的间隔相等，所以，项目之间的间隔比项目与边框的间隔大一倍。

  


  





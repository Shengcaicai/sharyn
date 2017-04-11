可以通过Image对象的complete 属性来检测图像是否加载完成

* 每个Image对象都有一个complete属性，当图像处于装载过程中时，该属性值false,当发生了onload、onerror、onabort中任何一个事件后，则表示图像装载过程结束（不管成没成功），此时complete属性为true
* |  |
  | :--- |


  |  | var img = new Image\(\); |
  | :--- | :--- |
  |  |  img.src = oImg\[0\].src = this.src.replace\(/small/,"big"\); |
  | 鼠标划过时，oDiv图像展示 |  oDiv.style.display = "block"; |
  |  |  |
  | 图片加载完成时，oDiv图像隐藏； |  img.complete ? oDiv.style.display = "none" : \(oImg\[0\].onload = function\(\) {oDiv.style.display = "none"}\) |
  |  |  |
  |  |  |




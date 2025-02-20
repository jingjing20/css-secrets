# CSS 揭秘

## 背景和边框
- [半透明边框](./background-border/translucent-borders.html)：默认情况下，背景会延伸到边框所在的区域下面，可以通过 **background-clip** 属性来调整默认行为。
- [多重边框](./background-border/multiple-borders.html)：使用 **box-shadow** 来模拟外框，模拟的边框出现在在外圈，并不会响应鼠标事件，可以给 **box-shadow** 属性加上 **inset** 关键字，来使投影绘制在元素的内圈。
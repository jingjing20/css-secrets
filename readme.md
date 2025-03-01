# CSS 揭秘

## 背景和边框

- [半透明边框](./background-border/translucent-borders.html)：默认情况下，背景会延伸到边框所在的区域下面，可以通过 **background-clip** 属性来调整默认行为。

- [多重边框](./background-border/multiple-borders.html)：使用 **box-shadow** 来模拟外框，模拟的边框出现在在外圈，并不会响应鼠标事件，可以给 **box-shadow** 属性加上 **inset** 关键字，来使投影绘制在元素的内圈。

- [灵活的背景定位](./background-border/extended-bg-position.html)：**background-position** 允许指定背景图片距离任意角的偏移量，只要在偏移量前面指定关键词。

- [灵活的背景定位](./background-border/background-origin.html)：默认情况下，**background-position** 是以 **padding-box** 为准的，可以使用 **background-origin** 来改变该基准。

- [灵活的背景定位](./background-border/background-position-calc.html)：使用calc()函数计算偏移值进行背景定位。

- [边框内圆角](./background-border/inner-rounding.html)：利用描边 **outline**不跟着圆角走的事实，配合 **box-shadow** 实现边框内圆角。

- [条纹背景-水平条纹](./background-border/horizontal-stripes.html)：使用线性渐变 **linear-gradient** 将两个色标重合可以创建实色条纹。如果某个色标的位置值比整个列表中在它之前的色标值都要小，则该色标的位置值会被设置成它前面所有色标位置的最大值。这意味着，如果把第二个色标的位置设置为0，那它的位置就总是被浏览器调整为前一个色标的位置值。

- [条纹背景-垂直条纹](./background-border/vertical-stripes.html)：垂直条纹的代码跟水平条纹几乎是一样的，差别主要在于:我们需要在 开头加上一个额外的参数来指定渐变的方向。

- [条纹背景-斜向条纹](./background-border/diagonal-stripes.html)：斜向条纹不但能简单通过改变渐变方向得到，原因在于只是把每个“贴片”内部渐变旋转了45度，而不是把整个重复的背景都旋转了。单个贴片包 含了四条条纹，而不是两条，只有这样才有可能做到无缝拼接。

- [条纹背景-更好的斜向条纹](./background-border/diagonal-stripes-60deg.html)：利用 **repeating-linear-gradient** 可以轻易实现任意角度的斜向条纹。

- [条纹背景-更好的斜向条纹](./background-border/test-color-stop-2positions.html)：利用 **repeating-linear-gradient** 可以在同一个色标上指定两个位置值相当于两个连续的色标具有相同的颜色和不同的位置，这个特性在创建渐变图案时是十分有用的。

- [灵活的同色系条纹](./background-border/subtle-stripes.html)：最深的颜色指定为背景色，同时把半透明白色的条纹叠加在背景色之上来 得到浅色条纹。

- [复杂的背景图案](./background-border/blueprint.html)：水平渐变图案跟垂直渐变图案配合实现简单的蓝图网格图案。

- [波点](./background-border/polka.html)：径向渐变创建最简单的圆点的阵列。

- [棋盘](./background-border/checkerboard.html)：用两个直角三角形来拼合出方块。

- [棋盘](./background-border/checkerboard-svg.html)：用 SVG 来实现棋盘效果。

- [伪随机背景](./background-border/cicada-stripes.html)：通过质数来增加随机真实性。

- [连续的图像边框](./background-border/border-image.html)：**border-image** 基本原理就是九宫格伸缩法：把图片切割成九块，然后把它们应用到元素边框相应的边和角。

- [连续的图像边框](./background-border/continuous-image-borders.html)：**border-image** 基本原理就是九宫格伸缩法：把图片切割成九块，然后把它们应用到元素边框相应的边和角。

- [老式信封样式边框](./background-border/vintage-envelope.html)：利用渐变实现老式信封样式边框。

- [蚂蚁行军边框](./background-border/marching-ants.html)：虚线边框动画。

- [脚注](./background-border/footnote.html)：脚注。

## 形状

- [自适应的椭圆](./shape/ellipse.html)：**border-radius** 可以单独指定水平和垂直半径，只要用一个斜杠（/）分隔这两个值即可。这个特性允许在拐角处创建椭圆圆角。

- [半椭圆](./shape/half-ellipse.html)

- [四分之一椭圆](./shape/quarter-ellipse.html)

- [平行四边形](./shape/parallelograms.html)：通过 skew 的变形属性对矩形进行拉伸。

- [平行四边形](./shape/parallelograms-pseudo.html)：利用伪元素以及定位属性产生一个方块，然后对伪元素设置样式，并将其放置在其宿主元素下层。当想变形一个元素而不想变形它对内容时非常有用。

- [菱形图片](./shape/diamond-images.html)：通过 rotate 变形 + scale 变形实现菱形图片，旋转后图片的宽度应与容器对角线相等。

- [菱形图片-裁剪路径](./shape/diamond-clip.html)：**clip-path** 属性可以把元素裁剪成任何形状。

- [切角效果](./shape/bevel-corners-gradients.html)：利用线性渐变实现切角效果。

- [切角效果](./shape/bevel-corners.html)：利用 SVG 实现切角效果。

- [切角效果](./shape/bevel-corners-clipped.html)：利用 **clip-path** 实现切角效果。

- [弧形切角](./shape/scoop-corners.html)：利用径向渐变实现弧形切角。
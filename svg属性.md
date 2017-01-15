# svg 自身属性：
* >svg画布的原点坐标试左上角，右x值为正向变大，下y值正向变大
>1.viewport:用width：100 svg画布宽度 height：200 svg画布高度，来设置可视区域大小。width height可以有单位，默认为像素px
>1.viewBox（x,y,width,height）：(0,0,100,200)从svg坐标位置0，0起，取宽高为100，200的矩形，填充满整个svg大小。该属性可以缩放移动svg图形。
>1.preserveAspectRatio：设置viewport宽高比与viewbox宽高比的比是否一致。
preserveAspectRatio=‘xMidYMid meet’：第1个值表示，viewBox如何与SVG viewport对齐；第2个值表示，如何维持高宽比（如果有）
第一个值选项：
值	   含义
xMin	viewport和viewBox左边对齐
xMid	viewport和viewBox x轴中心对齐
xMax	viewport和viewBox右边对齐
YMin	viewport和viewBox上边缘对齐。注意Y是大写。
YMid	viewport和viewBox y轴中心点对齐。注意Y是大写。
YMax	viewport和viewBox下边缘对齐。注意Y是大写。
第二个值含义：
值	    含义
meet	保持纵横比缩放viewBox适应viewport。（默认）根据宽高值较小一方缩放
slice	保持纵横比同时比例小的方向放大填满viewport。根据宽高值较大的一方缩放，超出的裁掉。
none	扭曲纵横比以充分适应viewport。

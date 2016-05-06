# RoundImage
##自定义圆形图片控件
##原理：
这次用的方法主要是通过BitmapShader来实现，Shader是颜色填充器，比如画了个圆，如果设置了Shader，且设置Shader颜色为蓝色，则画出的圆内部就会被蓝色填充。而BitmapShader则是用图片来作为填充物，因此，我们将需要处理的图片放入BitmapShader中，然后画一个圆，然后就会用之前的图像填充圆内部，然后就实现了圆形图片。同理也可以实现圆角矩形图片等效果。

##控件功能：
*1.根据画布大小，缩放处理的图片

*2.提供两种模式：

  -AUTO模式，将画布大小作为圆形半径
  
  -MANUAL模式，手动设置圆形半径，截取图片居中部分，不影响画布大小
  
##控件效果：
![doodles](http://img.blog.csdn.net/20160506152502717?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

具体步骤和之前自定义控件的差不多，源码里进行了注释，直接看源码就行。

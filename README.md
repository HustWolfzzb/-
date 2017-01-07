#开篇语
>笔者最近在做课程设计，已经经过了**  选题--分析--草图阶段   **了。明天进入**  绘制简图阶段  **  ，后天预计进入**  设计零件+结构  **  阶段，我的工作任务是**    寻找资料+计算机绘图+三维模型设计+动画制作+maybe a little 策划书工作**。Github是神器，所以我把内容都更新在Github上了，详情请参见。不大不小也是个项目吗。所以有兴趣的同学可以实时追踪。反正也不是啥申请专利的东西。放出来给大家做借鉴也是好的。Geek是不会介意资料外泄的~~


#正文
  >本文是我复习Solidworks的练手之作，旨在给大家介绍技术。并非是完整的项目的内容，具体项目见此[https://github.com/HustWolfzzb/Automatic-vegetable-cutting-machine](https://github.com/HustWolfzzb/Automatic-vegetable-cutting-machine)

>我仅仅是做出了一个模型，有关于solidworks的运动模型设计以及关于零件的设计与装配！


#####First 建模
![Solidworks--建模工具](http://upload-images.jianshu.io/upload_images/3810775-b7eb0fa02952992c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
>画出如下的零件

![如图为齿轮，随手画，不是确切的数据](http://upload-images.jianshu.io/upload_images/3810775-3cba5ca2989d260c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![如图为轴，随手画，不是确切的数据](http://upload-images.jianshu.io/upload_images/3810775-1f0c757cebb22202.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

##### Second 装配
>装配如图，简单的几个配合下去就好了，重点介绍下齿轮的配合

![配合如图](http://upload-images.jianshu.io/upload_images/3810775-682549aca435b656.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

>重要的提示：不要迷信网上的那些视频教程什么的一些麻烦的齿轮配合关系，如果你不是专业制作的，那用的着那么仔细？只要选择配合--机械配合--配合选择下，选择两个齿轮的中见面，告诉solidworks这个地方放个齿轮，然后设置一下传动比例就好了。另外，选中零件右键，找到浮动或者固定，让一个固定，然后另一个浮动。这样就可以有了基本的配合关系

![E(536X25N}$KX72D)]GO8GF.png](http://upload-images.jianshu.io/upload_images/3810775-be318229ee2df110.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#####Third 运动
>看到这里的运动算例，这个地方就是分管运动模型的建立的~选中，


![看到这里的运动算例，这个地方就是分管运动模型的建立的~~](http://upload-images.jianshu.io/upload_images/3810775-1325aa732ade43d8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


>找到马达选项，然后添加一个马达，左边上面是属性，找到你设置的浮动的那个齿轮，给定运动速度。

![找到马达选项，然后添加一个马达，左边上面是属性，找到你设置的浮动的那个齿轮，给定运动速度。](http://upload-images.jianshu.io/upload_images/3810775-97db104f5ff7ad48.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


>效果见图

![运动效果图](http://upload-images.jianshu.io/upload_images/3810775-8f64d00003a0007a.gif?imageMogr2/auto-orient/strip)


#结束语
>笔者很开心可以和大家分享自己的所见所知！有需求有兴趣的伙伴可以找我一起交流，虽然我也不是很熟练，但是人多力量大这点我还是知道的。come on ！！~~

#个人宣言
>知识传递力量，技术无国界，文化改变生活！

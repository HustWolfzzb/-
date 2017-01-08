![镇文神图](http://upload-images.jianshu.io/upload_images/3810775-1587e9dc0fe78c57.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#开篇语
>笔者最近在做课程设计，已经经过了**  选题--分析--草图阶段   **了。今天进入**  绘制简图阶段+设计零件+结构  **  阶段，我的工作任务是**    寻找资料+计算机绘图+三维模型设计+动画制作**。Github是神器，所以我把内容都更新在Github上了，详情请参见正文开头网址。所以有兴趣的同学可以实时追踪。反正也不是啥申请专利的东西。放出来给大家做借鉴也是好的。Geek是不会介意资料外泄的~~


#正文
  >本文是我开始做Solidworks课设的开山之作，旨在给大家介绍技术，只有开头的槽轮拨盘部分。并非是完整的项目的内容，具体项目见此
[https://github.com/HustWolfzzb/Automatic-vegetable-cutting-machine](https://github.com/HustWolfzzb/Automatic-vegetable-cutting-machine)
每天都有更新

>我仅仅是做出了一个模型，有关于solidworks的运动模型设计以及关于零件的设计与装配！


#####First 建模
![Solidworks--建模工具](http://upload-images.jianshu.io/upload_images/3810775-b7eb0fa02952992c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
>**画出如下的零件**
>如图为拨盘，盘身直径140mm，圆心到拨动件的圆心的距离是80，高度均为10mm

![如图为拨盘，盘身直径140mm，圆心到拨动件的圆心的距离是80，高度均为10mm](http://upload-images.jianshu.io/upload_images/3810775-2db9ae977e1faf96.gif?imageMogr2/auto-orient/strip)
>如图为槽轮，轮身直径160mm，拨动槽宽为10mm，深度为60mm；内部带键槽直径20mm，键高4mm，宽4mm，边缘圆弧与拨盘外圆密切贴合

![如图为槽轮，轮身直径160mm，拨动槽宽为10mm，深度为60mm；内部带键槽直径20mm，键高4mm，宽4mm，边缘圆弧与拨盘外圆密切贴合](http://upload-images.jianshu.io/upload_images/3810775-fe8ea870cfb2858f.gif?imageMogr2/auto-orient/strip)

##### Second 装配
>装配如图，简单的几个配合下去就好了，重点介绍下齿轮的配合

![装配细节如图所示，至于更细节的不太好说，自行体悟~~~]VRJ`MT.png](http://upload-images.jianshu.io/upload_images/3810775-e0f9fd61f40c05a4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

>重要的提示：请记住，槽轮一定要配合好，千万不要发生碰撞！！！配合的时候不要考虑键槽配合，本体没有那么多的固定件，一旦完全约束，直接零件会飞--真的会飞。。另外，选中零件右键，找到浮动或者固定，让过程中不需要运动的零件固定（本实例中为两根轴，提供转动轴心），然后另外需要运动的零件保持浮动。这样就可以有了基本的运动配合关系。



#####Third 运动
>看到这里的运动算例，这个地方就是分管运动模型的建立的~选中，即可进入动画制作页面。


![看到这里的运动算例，这个地方就是分管运动模型的建立的~~](http://upload-images.jianshu.io/upload_images/3810775-1325aa732ade43d8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

>另外，今天我才发现我的Solidworks是有缺陷的，所以我在网上找了不少的办法修复Solidworks的插件



>找到马达选项，然后添加一个马达，左边上面是属性，找到你设置的浮动的那个拨盘，给定运动速度。另外还有一个实体接触，如果你没有开启motion那么对不起，不得那个实体接触会是灰色的，所以GG根本没法做仿真，跟昨天的那个简单的不一样，那个是基于机械配合的实体配合，这个是基于仿真的motion分析，完全不可同日而语~~~motion分析设置在后面

![Motion开启](http://upload-images.jianshu.io/upload_images/3810775-27b30ee0b5f035f3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![如果你没有开启motion那么对不起，不得那个实体接触会是灰色的，所以GG根本没法做仿真，跟昨天的那个简单的不一样，那个是基于机械配合的实体配合，这个是基于仿真的motion分析，完全不可同日而语](http://upload-images.jianshu.io/upload_images/3810775-dcc7e3e4db6443b0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



>效果见图

![槽轮.gif](http://upload-images.jianshu.io/upload_images/3810775-4bc1407f46686097.gif?imageMogr2/auto-orient/strip)



#####附：修复Solidworks，开启Toolbox设计库和Motion分析等功能
这个方法适用solidworks2012~2014版本 解决之道如下：  

>1.win+R打开运行，输入regedit进入注册表编辑器  

![win+R打开运行，输入regedit进入注册表编辑器  ](http://upload-images.jianshu.io/upload_images/3810775-6775b1bca96109aa.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

--------------
>2.在注册表中找到```HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\Installer```，若没有这个文件夹，右键 window文件夹建一个项，命名为Installer

![在注册表中找到```HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\Installer```，若没有这个文件夹，右键 window文件夹建一个项，命名为Installer](http://upload-images.jianshu.io/upload_images/3810775-6745e20b8e21a7e5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

--------------------

>3.在Installer上新建一个Dword值，32位即可，名字为“```RemappedElevatedProxiesPolicy```”，然后右键新建```RemappedElevatedProxiesPolicy```修改，设值为```1```




![$在Installer上新建一个Dword值，32位即可，名字为“```RemappedElevatedProxiesPolicy```”，然后右键新建```RemappedElevatedProxiesPolicy```修改，设值为```1```](http://upload-images.jianshu.io/upload_images/3810775-5af2e4aafaf05cb0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

-----------------

> 4.打开自己原来的安装包，```setup```，修复，单单修复solidworks即可 



![打开自己原来的安装包，```setup```，修复，单单修复solidworks即可 ](http://upload-images.jianshu.io/upload_images/3810775-527ab60d7f6000cc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

--------------

>5.修复完成后打开solidworks，可以发现工具-插件里的插件已经齐全了，toolbox也可以正常使用了，  



![修复完成后打开solidworks，可以发现工具-插件里的插件已经齐全了，toolbox也可以正常使用了，  
](http://upload-images.jianshu.io/upload_images/3810775-fa2636d2c16c606e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

-------------
>6.最后别忘了，将“RemappedElevatedProxiesPolicy”的值改为0，这个bug就修复了。接下里开心的使用焕然一新的Solidworks吧~~~


#结束语
>笔者很开心可以和大家分享自己的所见所知！有需求有兴趣的伙伴可以找我一起交流，虽然我也不是很熟练，但是人多力量大这点我还是知道的。come on ！！~~

#个人宣言
>知识传递力量，技术无国界，文化改变生活！

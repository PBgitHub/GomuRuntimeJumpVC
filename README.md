# GomuRuntimeJumpVC

万能控制器跳转

在开发项目中，可能会遇到这样变态的需求：

推送：根据服务端推送过来的数据规则，跳转到对应的控制器。

最开始的想法是，写个switch，考虑所有的跳转因素，缺陷：如果有新需求跳转未在switch中的跳转因素需要发版本。

偶然翻看Runtime，发现可以利用runtime动态生成对象、属性、方法这特性。那么就开干。

1、根据推送规则跳转对应界面

![image](https://github.com/PBgitHub/MyImage/raw/master/git_Image/GomuRuntimeJumpImage/GomuRuntimeJumpImage1.png)

2、推送过来的消息规则
模拟服务器返回的数据：

![image](https://github.com/PBgitHub/MyImage/raw/master/git_Image/GomuRuntimeJumpImage/GomuRuntimeJumpImage2.png)

3、跳转界面

![image](https://github.com/PBgitHub/MyImage/raw/master/git_Image/GomuRuntimeJumpImage/GomuRuntimeJumpImage3.png)

4、检测对象是否存在该属性

![image](https://github.com/PBgitHub/MyImage/raw/master/git_Image/GomuRuntimeJumpImage/GomuRuntimeJumpImage4.png)

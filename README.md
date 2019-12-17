# LiverHolo
An Hololens App for Moving, Scaling and Rotating a liver model

## 配置：
1. Hololens 1st；
2. windows 10 非家庭版: 开启“Hyper-V”，以及“开发者模式”；
3. visual studio 2017: 2019不兼容；
4. uwp sdk 10.0.17763.134: 高版本不兼容，可以和vs2017一起下载；
5. unity 5.6.1: 添加场景，build setting - 切换平台到uwp，target device为Hololens，勾选unity C# projects*，player setting - other setting - 勾选 Virtual Reality Supporter - 设置为Windows Mixed Reality；
6. HoloToolkit 2017版: 高版本不兼容；
7. TransformKit: https://github.com/pampas93/RotateScale_Hololens
8. Hololens Emulator: 第一代；

## 调试：
1. vs2017打开sln文件；
2. debug + x86 + Hololens Emulator；

## Debug：
1. 模型的每一部分都要在CAD文件里设置轴居中到对象然后导出fbx文件；
2. *.dll文件缺失，将project.lock.json中的10.0.*为10.0，参考下文：https://forums.hololens.com/discussion/8382/hololens-universal10-build-json-dll-error-solve#latest

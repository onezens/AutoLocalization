# AutoLocalization
Auto Localization for xib and storyboard(xib和storyboard自动添加国际化)

#注意
Swift和OC项目都可以使用

#用法
  1. 将存放脚本文件的文件夹，导入脚本文件到项目的`根目录`
  2. 选择项目 -> targes -> Build Phases -> + -> New Run Script Phase
  3. 添加两个运行脚本，其中一个添加脚本`python ${SRCROOT}/${TARGET_NAME}/RunScript/AutoGenStringsSB.py ${SRCROOT}/${TARGET_NAME}`, 另一个添加`python ${SRCROOT}/${TARGET_NAME}/RunScript/AutoGenStringsXIB.py ${SRCROOT}/${TARGET_NAME}`
  4. Build Setting  ->  Deployment  -> Deployment Location / Deployment Postprocessing  -> Yes
  5. 分别创建一个xib和storyboard，然后开启国际化后，添加控件，Command + B 后查看你的国际化文件
  
  ![](http://7xq8l3.com1.z0.glb.clouddn.com/AutoLocalization1.png)
  
  ![](http://7xq8l3.com1.z0.glb.clouddn.com/AutoLocalization2.png)
  
#效果图
![](http://7xq8l3.com1.z0.glb.clouddn.com/autoLocalizationDemo.gif)
  
# 缺点
  1. xib 和storyboard文件只能保存在根目录
  2. xib 和 storyboard 文件功能相同但是在不同的文件中
  3. 文件路径中不能拥有空格，否则Xcode脚本会找不到文件的错误
# 求大神修改
本文最初地址：[http://www.cnblogs.com/levilinxi/p/4296712.html](http://www.cnblogs.com/levilinxi/p/4296712.html)
  



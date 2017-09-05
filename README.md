# AutoLocalization

xib和storyboard自动国际化

[查看自动国际化脚本](https://github.com/onezens/AutoLocalization/blob/master/AutoLocalization/RunScript/AutoGenStrings.py)

## 脚本升级记录  
 
 
 1. 2017.06.02 自动化脚本在原先作者的基础上进行修改，现在同一个文件，支持xib和storyboard的一次性国际化
 2. 2017.8.10 遍历项目根目录下所有xib、storyboard文件并且国际化

## 用法
  1. 将存放脚本文件的文件夹，导入脚本文件到项目的`根目录`
  2. 选择项目 -> targes -> Build Phases -> + -> New Run Script Phase
  3. 添加两个运行脚本，其中一个添加脚本`python ${SRCROOT}/${TARGET_NAME}/RunScript/AutoGenStrings.py ${SRCROOT}/${TARGET_NAME}`
  4. Build Setting  ->  Deployment  -> Deployment Location / Deployment Postprocessing  -> Yes
  5. 分别创建一个xib和storyboard，然后开启国际化后，添加控件，Command + B 后查看你的国际化文件
  
  ![](http://7xq8l3.com1.z0.glb.clouddn.com/AutoLocalization1.png)
  
  ![](http://upload-images.jianshu.io/upload_images/1216462-9f20ceca2e58bebb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
  
## 效果图
![](http://upload-images.jianshu.io/upload_images/1216462-c6978ae9c7814094.gif?imageMogr2/auto-orient/strip)

## 国际化详解博客
[http://www.jianshu.com/p/7e1c7c210ec2](http://www.jianshu.com/p/7e1c7c210ec2)

## 注意
文件路径中不能拥有空格，否则Xcode脚本会找不到文件的错误

## 脚本来源
[http://www.cnblogs.com/levilinxi/p/4296712.html](http://www.cnblogs.com/levilinxi/p/4296712.html)

  

  



# 华为分析服务Android SDK示例代码


## 目录

* [简介](#简介)
* [快速入门](#快速入门)
* [安装](#安装)
* [配置](#配置)
* [环境要求](#环境要求)
* [操作结果](#操作结果)
* [授权许可](#授权许可)


## 简介
Hmsanalyticskitdemo提供了华为分析服务（HUAWEI Analytics Kit）与app集成的示例代码。其演示了如何通过收集预定义事件和自定义事件以提高用户参与度和用户偏好。[了解更多有关Analytics Kit的信息](https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/introduction-0000001050745149)。

该示例也可以通过HMS Toolkit快速启动运行，且支持各Kit一站式集成，并提供远程真机免费调测等功能。了解更多信息，请参考[HMS Toolkit官方链接](https://developer.huawei.com/consumer/cn/doc/development/Tools-Guides/getting-started-0000001077381096)。

## 快速入门

更多开发指导，请参考以下链接文档：

[开发指南](https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/android-dev-process-0000001050163813)。

[API参考](https://developer.huawei.com/consumer/cn/doc/development/HMSCore-References/android-api-analytics-overview-0000001051067140)。

Hmsanalyticskitdemo以Gradle构建系统为例演示了如何使用Android分析服务SDK。

首先，我们通过克隆此仓库或下载压缩包的方式来下载AnalyticsKit-master。

在Android Studio中，点击`Open an existing Android Studio project`，选择`Analytics_android_Java_Full`。

您可以直接运行gradle build命令构建工程。

您需要在AppGallery Connect中创建应用，获取`agconnect-services.json`文件，并将文件添加到项目中。[进一步了解开发流程](https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/android-dev-process-0000001050163813)。


## 安装
使用Android Studio打开解压后的工程。

## 配置
1. 在AppGallery Connect中创建应用，并获取项目配置文件agconnect-services.json。在Android Studio中，切换到Project视图，将agconnect-services.json文件移动到app的根目录下。 
2. 修改app的build.gradle文件中的applicationId为上一步申请的app包名。

## 环境要求
硬件要求：
1. 电脑（台式机或笔记本）
2. 华为手机，用于应用调试
  
软件要求：
1. 华为分析服务6.3.2
2. 适配Android 4.3 Jelly Bean（API level 18）及以上版本的设备
3. Android Studio 
4. JDK 1.8及以上

## 操作结果
运行该app后，您将会看到如下页面：

<img src="./images/screen_0.PNG" height="534" width="300" style="max-width:100%;">

点击“TRUE”或“FALSE” 按钮进行答题；点击“NEXT” 按钮进入下一道题；点击“POST SCORE”按钮记录用户获得的分数。所有信息将被上传到Analytics Kit控制台，您可以使用Debug View实时查看这些信息。

点击SETTINGS按钮:

<img src="./images/screen_1.PNG" height="534" width="300" style="max-width:100%;">

当点击SETTINGS按钮，您会被要求提供最喜欢的运动。您的选择将作为用户属性记录到Analytics Kit中。

## 授权许可
HmsAnalyticsKitDemo经过[Apache 2.0授权许可](http://www.apache.org/licenses/LICENSE-2.0)。


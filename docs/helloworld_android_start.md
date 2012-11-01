开始android html5 应用开发
====================
## 1. Requirements
* jdk1.6： [下载](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* android sdk包： [下载](http://developer.android.com/sdk/index.html) ,安装后，通过sdk manager下载需要的sdk版本（目前可能需要设置goagent代理翻墙下载）
* Apache Cordova：用于转化html5 web app 为 手机端native app. [下载](http://phonegap.com/download)

## 2. 在IDEA下新建'helloworld'的android工程： IDEA已原生包含android插件，该步骤比较简单。
* 运行IDEA, 选择[File]->[New Project], 打开NEW project 窗口。
* 选择[create project from scratch], 点击next。
* 在新打开的窗口，填写或选择‘project name’、‘select project files location’、‘select type’项， 点击next。 界面如下图：
<br />
![程序截图](https://raw.github.com/sdg-sysdev/html5MoblieApp-study/master/docs/img/helloworld-1.jpg)  
* 在新打开的窗口，选择配置好'android sdk', 其他默认， 点击[finish]完成。 界面如下图：
<br />
![程序截图](https://raw.github.com/sdg-sysdev/html5MoblieApp-study/master/docs/img/helloworld-3.jpg) 
![程序截图](https://raw.github.com/sdg-sysdev/html5MoblieApp-study/master/docs/img/helloworld-2.jpg) 

## 3. 配置Apache Cordova框架的android插件到应用。该步骤可参考：[phonegap 文档](http://docs.phonegap.com/en/2.1.0/guide_getting-started_android_index.md.html#Getting%20Started%20with%20Android)
* In the root directory of your project, create two new directories:
* Copy cordova-2.0.0.js from your Cordova download earlier to assets/www
* Copy cordova-2.0.0.jar from your Cordova download earlier to /libs
* Edit your project's main Java file found in the src folder:
  Add import org.apache.cordova.*;
  Change the class's extend from Activity to DroidGap
  Replace the setContentView() line with super.loadUrl("file:///android_asset/www/index.html");

## 4A. 部署到模拟器
* 打开‘Run/debug configuration’， 选择‘target Device > Emulator ' ,  点击ok 完成。 界面如下图：
<br />
![程序截图](https://raw.github.com/sdg-sysdev/html5MoblieApp-study/master/docs/img/helloworld-4.jpg) 
* 点击运行helloworld 应用。 由于启动模拟器比较慢，请耐心等待，模拟器打开后界面如下：
<br />
![程序截图](https://raw.github.com/sdg-sysdev/html5MoblieApp-study/master/docs/img/helloworld-5.jpg) 

## 4B. 部署到android真机
* Make sure USB debugging is enabled on your device and plug it into your system. (Settings > Applications > Development)
* 打开‘Run/debug configuration’， 选择‘target Device > USB device ' ,  点击ok 完成。 界面如下图：
* 点击运行helloworld 应用。在手机上就能看到helloworld应用。

Done!








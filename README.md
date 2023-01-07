# flutter_demo

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## windows安装运行
- https://www.w3cschool.cn/evilg/evilg-ki6q35t5.html
- 编辑器： vscode
- flutter版本：Flutter 3.3.9 • channel stable, Dart 2.18.5 • DevTools 2.15.0
VisualStudio版本：Visual Studio Community 2022
androidStudio版本：Android studio Dolphin | 2021.3.1 Patch 1，Runtime version: 11.0.13+0-61751.21-8125866 amd64，VM: OpenJDK 64-Bit Server VM by JetBrains s.r.o.

```shell
    flutter doctor

    Doctor summary (to see all details, run flutter doctor -v):
    [√] Flutter (Channel stable, 3.3.9, on Microsoft Windows [版本
        10.0.19045.2311], locale zh-CN)
    [√] Android toolchain - develop for Android devices (Android SDK version    33.0.1)
    [√] Chrome - develop for the web
    [√] Visual Studio - develop for Windows (Visual Studio Community 2022   
        17.4.2)
    [√] Android Studio (version 2021.3)
    [√] IntelliJ IDEA Community Edition (version 2022.2)
    [√] Connected device (3 available)
    [√] HTTP Host Availability  
```
 ## Mac安装运行
 教程参考：https://flutter.cn/docs/get-started/install/macos#set-up-the-ios-simulator
 ```shell
flutter doctor
Doctor summary (to see all details, run flutter doctor -v):
[✓] Flutter (Channel stable, 3.3.10, on macOS 12.6.2 21G320 darwin-arm, locale
    zh-Hans-CN)
[✓] Android toolchain - develop for Android devices (Android SDK version 33.0.1)
[!] Xcode - develop for iOS and macOS (Xcode 14.2)
    ! CocoaPods 1.8.4 out of date (1.11.0 is recommended).
        CocoaPods is used to retrieve the iOS and macOS platform side's plugin
        code that responds to your plugin usage on the Dart side.
        Without CocoaPods, plugins will not work on iOS or macOS.
        For more info, see https://flutter.dev/platform-plugins
      To upgrade see
      https://guides.cocoapods.org/using/getting-started.html#installation for
      instructions.
[✓] Chrome - develop for the web
[✓] Android Studio (version 2021.3)
[✓] VS Code (version 1.74.2)
[✓] Connected device (3 available)
[✓] HTTP Host Availability
 ```
 - 安装 cocoapods 是会报错，直接安装低版本的 cocoapods 就可以了
  ```shell
    sudo gem install cocoapods -v 1.8.4
  ```
执行 open -a Simulator 打开XCode 模拟器，VScode 运行 flutter 项目，会直接在 模拟器中打开测试页面 Launching lib/main.dart on iPhone 14 Pro Max in debug mode...。

### 项目运行步骤
- 1.在本机上单独启动 android studio / XCode 的 emulator：  C:\Users\Administrator\AppData\Local\Android\Sdk\emulator\emulator.exe -avd Pixel_4XL_API_30_x86_64 ，桌面上放个快捷脚本 .bat
- 2.运行命令: flutter run

## 文件内容解析
- /lib/main.dart，运行时的主文件，里面有运行的入口函数
- 在pubspec.yaml文件，dependencies部分添加所依赖的库和版本，然后执行 flutter packages get 安装新的包依赖，并且在 pubspec.lock 中添加依赖版本信息


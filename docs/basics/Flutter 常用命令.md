# 1、检查 Flutter 开发环境

```
flutter doctor
```

用于检查开发环境是否满足 Flutter 开发的要求。它会自动检测并报告缺少的依赖项、配置错误等，帮助开发者确保开发环境的正确性和稳定性。

```
- flutter doctor -v
```
  
该命令的作用和 `flutter doctor` 命令基本一致，都是用来检查开发环境是否满足 Flutter 开发的要求。但是，`flutter doctor -v` 命令会提供更详细的输出，显示出每个问题的详细信息，以及每个已安装包的详细版本信息，可以帮助开发者更深入地了解具体的环境问题。

# 2、创建 Flutter 项目

```
flutter create <项目名称>
```

例如： flutter create my_app

```
flutter create --org com.example <项目名称>
```

创建一个包名为 com.example 的项目

```
flutter create --org com.example --platforms android,ios,macos,web <项目名称>
```

创建项目时配置支持的平台

# 3、查看 Flutter SDK 的版本号

```
flutter --version
```

# 4、清除 Flutter 构建缓存

```
flutter clean
```

# 5、获取 Dart Package 依赖项

```
flutter pub get
```

# 6、构建应用安装包

- Android

```
flutter build apk
```

该命令默认带有 --release 参数。

如果你想构建不同 ABI 的 APK 文件，可以使用 --split-per-abi 参数：

```
flutter build apk --split-per-abi
```

该命令会将应用安装包拆分为多个 APK 文件，每个 APK 文件对应一个 ABI（二进制接口），可以减少安装包的大小。

这个命令会生成如下三个 APK 文件：

[project]/build/app/outputs/apk/release/app-armeabi-v7a-release.apk
[project]/build/app/outputs/apk/release/app-arm64-v8a-release.apk
[project]/build/app/outputs/apk/release/app-x86_64-release.apk

参考：[构建和发布为 Android 应用](https://flutter.cn/docs/deployment/android)

- iOS

```
flutter build ipa
```

参考：[构建和发布为 iOS 应用](https://flutter.cn/docs/deployment/ios)

- macOS

```
flutter build macos
```

参考：[构建和发布为 macOS 应用](https://flutter.cn/docs/deployment/macos)

- Linux

参考：[Build the snap](https://flutter.cn/docs/deployment/linux#build-the-snap)

- windows

```
flutter build windows
```

参考：[构建和发布为 Windows 应用](https://flutter.cn/docs/deployment/windows)

- web

```
flutter build web
```

参考：[构建和发布为 Web 应用](https://flutter.cn/docs/deployment/web)


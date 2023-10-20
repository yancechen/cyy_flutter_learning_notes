Flutter 里除了提供基本的 widget library 外，还默认提供了两种风格的 widget 库，即 `Material widgets` 和 `Cupertino widgets`。

`Material widgets` 和 `Cupertino widgets` 都提供了大量的基础 widget，但它们的设计理念不同。

`Material widgets` 是基于 `Material Design` 设计风格的 widget 库，而 `Cupertino widgets` 是基于 `Apple Human Interface Guidelines` 实现了当前的 iOS 设计风格的 widget 库。

Material 设计风格是为**全平台**设计的，不仅仅只是 Android 。当你使用 Flutter 编写一个 Material 风格的 app 时，它运行在任何平台上都是有着 Material 的设计展示，即使是在 iOS 下。但是如果你想要让你的 app 更像标准的 iOS 风格的话，那你就需要用到 Cupertino 库了。

有一点需要注意，技术上来说，你可以在 iOS 和 Android 上正常运行一个 Cupertino 搭建的 app，但是（因为一些授权的原因），Cupertino 在 Android 上并不能展示它应有的字体。正因为此，当你编写一个 Cupertino app 的时候，你应该让其运行在 iOS 的设备上。



# 编译iOS 工程

还原一个iOS 工程的生成过程.
不使用 Xcode, 用最原始的方法编译一个 iOS ipa包. 越精简越好,用最少的配置和最少的代码 把一个 具有所有内容的 iOS 工程编译成一个 ipa 包.
entitlements.plist 权限文件只要最少的东西,能编译就行
工程的配置Info.plist 文件中的配置项只要能支撑一个 ipa 包在设备上运行就行
整个过程配置 和 代码越少,越能理解一个 iOS app 的生成过程

clang 编译参数
-fmodules      自动寻找到需要的系统库
-fobjc-arc     由ARC编译
-isysroot      指定系统SDK路径

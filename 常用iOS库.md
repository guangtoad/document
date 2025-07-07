# iOS开发库

## 目录
- [网络请求与通信](#网络请求与通信)
- [JSON 与模型映射](#json-与模型映射)
- [数据持久化](#数据持久化)
- [UI 组件与布局扩展](#ui-组件与布局扩展)
- [图片处理与缓存](#图片处理与缓存)
- [响应式编程](#响应式编程)
- [数据压缩与归档](#数据压缩与归档)
- [XML 解析](#xml-解析)
- [统计与分析](#统计与分析)
- [路由及-URL-处理](#路由及-url-处理)
- [内部自定义工具](#内部自定义工具)
- [图片与视频处理](#图片与视频处理)
- [HTML 解析](#html-解析)
- [日志管理](#日志管理)
- [Socket-与-实时通信](#socket-与-实时通信)
- [地图与导航](#地图与导航)
- [测试辅助工具](#测试辅助工具)
- [其他辅助工具](#其他辅助工具)

### 网络请求与通信

| 库名         | 官网                                                                                   | 简介                                   | 开源协议      | CocoaPods | SPM         |
| ------------ | -------------------------------------------------------------------------------------- | -------------------------------------- | ------------- | --------- | ----------- |
| AFNetworking | [github.com/AFNetworking/AFNetworking](https://github.com/AFNetworking/AFNetworking)    | iOS/OS X 网络请求库                    | MIT           | 支持      | 支持（v4.0.1+） |
| Alamofire    | [github.com/Alamofire/Alamofire](https://github.com/Alamofire/Alamofire)                 | Swift 网络请求库                       | MIT           | 支持      | 支持        |
| Moya         | [github.com/Moya/Moya](https://github.com/Moya/Moya)                                     | 基于 Alamofire 的 API 抽象层              | MIT           | 支持      | 支持        |

---

### JSON 与模型映射

| 库名         | 官网                                                                                             | 简介                                   | 开源协议 | CocoaPods | SPM    |
| ------------ | ------------------------------------------------------------------------------------------------ | -------------------------------------- | -------- | --------- | ------ |
| MJExtension  | [github.com/CoderMJLee/MJExtension](https://github.com/CoderMJLee/MJExtension)                   | 模型与 JSON/字典转换工具                | MIT      | 支持      | 不支持 |
| YYModel      | [github.com/ibireme/YYModel](https://github.com/ibireme/YYModel)                                 | 高性能 JSON 与模型转换库                | MIT      | 支持      | 不支持 |
| ObjectMapper | [github.com/tristanhimmelman/ObjectMapper](https://github.com/tristanhimmelman/ObjectMapper)     | Swift 对象与 JSON 映射                   | MIT      | 支持      | 未知   |
| HandyJSON    | [github.com/alibaba/HandyJSON](https://github.com/alibaba/HandyJSON)                             | Swift 轻量级 JSON 映射库                 | MIT      | 支持      | 未知   |
| ProtocolBuffers | [github.com/alexeyxo/protobuf-objc](https://github.com/alexeyxo/protobuf-objc)                 | Protocol Buffers 的 Objective-C 实现     | BSD      | 支持      | 不支持 |
| JSONKit      | [github.com/johnezang/JSONKit](https://github.com/johnezang/JSONKit)                             | 高性能 JSON 解析库                      | BSD      | 支持      | 不支持 |
| KakaJSON     | [github.com/KakaJSON/KakaJSON](https://github.com/KakaJSON/KakaJSON)                             | Swift 高性能 JSON 转模型库               | MIT      | 支持      | 未知   |
| SwifterSwift | [github.com/SwifterSwift/SwifterSwift](https://github.com/SwifterSwift/SwifterSwift)             | 常用 Swift 扩展工具集合                  | MIT      | 支持      | 支持   |

---

### 数据持久化

| 库名         | 官网                                                                              | 简介                                   | 开源协议            | CocoaPods | SPM    |
| ------------ | --------------------------------------------------------------------------------- | -------------------------------------- | ------------------- | --------- | ------ |
| Realm        | [realm.io](https://realm.io)                                                      | 跨平台移动数据库解决方案                | Apache License 2.0  | 支持      | 支持   |
| RealmSwift   | [realm.io/docs/swift/latest/](https://realm.io/docs/swift/latest/)                  | Realm 的 Swift 封装                     | Apache License 2.0  | 支持      | 支持   |
| FMDB         | [github.com/ccgus/fmdb](https://github.com/ccgus/fmdb)                            | SQLite 的 Objective-C 封装库             | BSD/MIT             | 支持      | 不支持 |
| SQLite.swift | [github.com/stephencelis/SQLite.swift](https://github.com/stephencelis/SQLite.swift) | SQLite 在 Swift 中的封装                | MIT                 | 支持      | 支持   |
| FCModel      | [github.com/FullDecent/FCModel](https://github.com/FullDecent/FCModel)              | ORM 数据模型库                          | MIT                 | 支持      | 不支持 |

---

### UI 组件与布局扩展

| 库名                     | 官网                                                                                                 | 简介                                       | 开源协议            | CocoaPods | SPM    |
| ------------------------ | ---------------------------------------------------------------------------------------------------- | ------------------------------------------ | ------------------- | --------- | ------ |
| UITextView+Placeholder   | [github.com/ryanmaxwell/UITextView-Placeholder](https://github.com/ryanmaxwell/UITextView-Placeholder) | UITextView 扩展，支持 placeholder 功能         | MIT                 | 支持      | 不支持 |
| Toast                    | [github.com/scalesec/Toast](https://github.com/scalesec/Toast)                                       | 快速展示 Toast 消息提示                      | MIT                 | 支持      | 不支持 |
| MJRefresh                | [github.com/CoderMJLee/MJRefresh](https://github.com/CoderMJLee/MJRefresh)                           | 下拉刷新控件                               | MIT                 | 支持      | 不支持 |
| FLAnimatedImage          | [github.com/Flipboard/FLAnimatedImage](https://github.com/Flipboard/FLAnimatedImage)                   | 高效 GIF 动画播放控件                        | MIT                 | 支持      | 不支持 |
| iCarousel                | [github.com/nicklockwood/iCarousel](https://github.com/nicklockwood/iCarousel)                       | 轮播展示控件                               | MIT                 | 支持      | 不支持 |
| JMDropMenu               | [github.com/Yalantis/JMDropMenu](https://github.com/Yalantis/JMDropMenu)                             | 下拉菜单控件                               | MIT                 | 支持      | 不支持 |
| IQDropDownTextField      | [github.com/hackiftekhar/IQDropDownTextField](https://github.com/hackiftekhar/IQDropDownTextField)     | 下拉选择输入框控件                          | MIT                 | 支持      | 不支持 |
| BetterSegmentedControl   | [github.com/halbou/BetterSegmentedControl](https://github.com/halbou/BetterSegmentedControl)         | 自定义分段控件                              | MIT                 | 支持      | 支持   |
| DZNEmptyDataSet          | [github.com/dzenbot/DZNEmptyDataSet](https://github.com/dzenbot/DZNEmptyDataSet)                     | 列表控件空数据占位视图                       | MIT                 | 支持      | 不支持 |
| Lottie                   | [github.com/airbnb/lottie-ios](https://github.com/airbnb/lottie-ios)                                 | 播放基于 JSON 描述的矢量动画                   | Apache License 2.0  | 支持      | 支持   |
| Charts                   | [github.com/danielgindi/Charts](https://github.com/danielgindi/Charts)                               | 多平台图表绘制库                           | MIT                 | 支持      | 支持   |
| SnapKit                  | [github.com/SnapKit/SnapKit](https://github.com/SnapKit/SnapKit)                                     | Swift AutoLayout DSL 框架                  | MIT                 | 支持      | 支持   |
| Masonry                  | [github.com/SnapKit/Masonry](https://github.com/SnapKit/Masonry)                                     | Objective-C AutoLayout 链式封装              | MIT                 | 支持      | 不支持 |
| PureLayout               | [github.com/PureLayout/PureLayout](https://github.com/PureLayout/PureLayout)                         | 简化 AutoLayout 设置                        | MIT                 | 支持      | 未知   |
| TPKeyboardAvoiding       | [github.com/michaeltyson/TPKeyboardAvoiding](https://github.com/michaeltyson/TPKeyboardAvoiding)       | 处理键盘遮挡问题                           | MIT                 | 支持      | 不支持 |
| IQKeyboardManager        | [github.com/hackiftekhar/IQKeyboardManager](https://github.com/hackiftekhar/IQKeyboardManager)         | 自动管理键盘，防止遮挡输入框                  | MIT                 | 支持      | 支持   |
| JDStatusBarNotification  | [github.com/samvermette/JDStatusBarNotification](https://github.com/samvermette/JDStatusBarNotification) | 状态栏提示通知控件                          | MIT                 | 支持      | 不支持 |
| MSDynamicsDrawerViewController | [github.com/mikefrederick/MSDynamicsDrawerViewController](https://github.com/mikefrederick/MSDynamicsDrawerViewController) | 侧边抽屉导航控制器                          | MIT                 | 支持      | 不支持 |
| WebViewJavascriptBridge  | [github.com/marcuswestin/WebViewJavascriptBridge](https://github.com/marcuswestin/WebViewJavascriptBridge) | JS 与原生代码通信桥接                        | MIT                 | 支持      | 不支持 |

---

### 图片处理与缓存

| 库名       | 官网                                                                                    | 简介                        | 开源协议 | CocoaPods | SPM    |
| ---------- | --------------------------------------------------------------------------------------- | --------------------------- | -------- | --------- | ------ |
| SDWebImage | [github.com/SDWebImage/SDWebImage](https://github.com/SDWebImage/SDWebImage)             | 异步图片下载与缓存           | MIT      | 支持      | 支持  |
| Kingfisher | [github.com/onevcat/Kingfisher](https://github.com/onevcat/Kingfisher)                   | Swift 图片下载与缓存库       | MIT      | 支持      | 支持  |

---

### 响应式编程

| 库名              | 官网                                                                                     | 简介                                     | 开源协议 | CocoaPods | SPM    |
| ----------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------- | -------- | --------- | ------ |
| ReactiveObjC      | [github.com/ReactiveCocoa/ReactiveObjC](https://github.com/ReactiveCocoa/ReactiveObjC)       | Objective-C 响应式编程框架                | MIT      | 支持      | 支持?（最新版本需查阅） |
| ReactiveCocoa     | [github.com/ReactiveCocoa/ReactiveCocoa](https://github.com/ReactiveCocoa/ReactiveCocoa)      | 跨平台响应式编程库                        | MIT      | 支持      | 支持?（最新版本需查阅） |
| RxSwift           | [github.com/ReactiveX/RxSwift](https://github.com/ReactiveX/RxSwift)                         | Swift 版响应式编程库                      | MIT      | 支持      | 支持  |
| ReactiveObjCBridge| （详见 ReactiveCocoa 项目）                                                               | Objective-C 与 ReactiveCocoa 桥接工具       | MIT      | 支持      | 未知   |

---

### 数据压缩与归档

| 库名     | 官网                                                                                      | 简介                      | 开源协议 | CocoaPods | SPM    |
| -------- | ----------------------------------------------------------------------------------------- | ------------------------- | -------- | --------- | ------ |
| GZIP     | [github.com/nicklockwood/GZIP](https://github.com/nicklockwood/GZIP)                        | 数据压缩/解压工具          | MIT      | 支持      | 不支持 |
| ZipArchive | [github.com/ZipArchive/ZipArchive](https://github.com/ZipArchive/ZipArchive)               | ZIP 文件压缩与解压工具      | MIT      | 支持      | 不支持 |

---

### XML 解析

| 库名    | 官网                                                                                   | 简介                         | 开源协议             | CocoaPods | SPM    |
| ------- | -------------------------------------------------------------------------------------- | ---------------------------- | -------------------- | --------- | ------ |
| KissXML | [github.com/robbiehanson/KissXML](https://github.com/robbiehanson/KissXML)             | 基于 NSXML 的 XML 解析库       | Apache License 2.0   | 支持      | 不支持 |

---

### 统计与分析

| 库名                 | 官网                                        | 简介                                   | 开源协议 | CocoaPods | SPM    |
| -------------------- | ------------------------------------------- | -------------------------------------- | -------- | --------- | ------ |
| PiwikTracker/Matomo  | [matomo.org](https://matomo.org)            | 网站/应用访问统计与数据分析工具          | GPL v3   | 支持      | 不支持 |

---

### 路由及 URL 处理

| 库名         | 官网                                                                                 | 简介                           | 开源协议 | CocoaPods | SPM    |
| ------------ | ------------------------------------------------------------------------------------ | ------------------------------ | -------- | --------- | ------ |
| MGJRouter    | [github.com/meili/MGJRouter](https://github.com/meili/MGJRouter)                     | 应用内 URL 路由与跳转管理         | MIT      | 支持      | 不支持 |
| FFRouter     | [github.com/ibireme/FFRouter](https://github.com/ibireme/FFRouter)                   | URL 路由管理框架                | MIT      | 支持      | 不支持 |
| FNUrlRoute   | 无公开官网                                                                           | URL 路由工具（类似 MGJRouter）    | 未知     | 支持?     | 未知   |
| TGRouteSwift | 本地依赖                                                                             | 内部 Swift 路由框架              | 未知     | 支持?     | 未知   |

---

### 内部/自定义工具 (本地依赖)

| 库名         | 官网    | 简介                     | 开源协议 | CocoaPods | SPM    |
| ------------ | ------- | ------------------------ | -------- | --------- | ------ |
| TGFoundation | 本地依赖| 内部基础工具库           | 未知     | 支持?     | 未知   |
| TGRouler    | 本地依赖| 内部工具组件             | 未知     | 支持?     | 未知   |
| TGLog       | 本地依赖| 内部日志记录库           | 未知     | 支持?     | 未知   |
| TGSQLiteHelper | 本地依赖 | 内部 SQLite 操作辅助库 | 未知     | 支持?     | 未知   |
| TGFileUtil  | 本地依赖| 内部文件操作工具库       | 未知     | 支持?     | 未知   |
| TGUIKit     | 本地依赖| 内部 UI 组件库            | 未知     | 支持?     | 未知   |
| ReaderCardID| 本地依赖| 内部身份读卡工具库        | 未知     | 支持?     | 未知   |

---

### 图片与视频处理

| 库名           | 官网                                                                                 | 简介                                | 开源协议       | CocoaPods | SPM    |
| -------------- | ------------------------------------------------------------------------------------ | ----------------------------------- | -------------- | --------- | ------ |
| OpenCV         | [opencv.org](https://opencv.org)                                                     | 计算机视觉与图像处理库               | BSD            | 支持?     | 未知   |
| TesseractOCRiOS| [github.com/gali8/Tesseract-OCR-iOS](https://github.com/gali8/Tesseract-OCR-iOS)         | iOS OCR（光学字符识别）封装          | Apache License 2.0 | 支持  | 不支持 |

---

### HTML 解析

| 库名       | 官网                                                                                     | 简介                      | 开源协议 | CocoaPods | SPM    |
| ---------- | ---------------------------------------------------------------------------------------- | ------------------------- | -------- | --------- | ------ |
| HTMLReader | [github.com/nolanw/HTMLReader](https://github.com/nolanw/HTMLReader)                      | HTML 文档解析工具         | MIT      | 支持      | 不支持 |

---

### 日志管理

| 库名              | 官网                                                                                             | 简介                                | 开源协议           | CocoaPods | SPM    |
| ----------------- | ------------------------------------------------------------------------------------------------ | ----------------------------------- | ------------------ | --------- | ------ |
| CocoaLumberjack | [github.com/CocoaLumberjack/CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)   | 高性能日志记录库                     | Apache License 2.0 | 支持      | 支持  |
| Log4swift        | [github.com/onmyway133/Log4swift](https://github.com/onmyway133/Log4swift)                       | Swift 日志记录库                    | MIT                | 支持      | 未知   |

---

### Socket 与实时通信

| 库名              | 官网                                                                                                 | 简介                            | 开源协议 | CocoaPods | SPM    |
| ----------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------- | -------- | --------- | ------ |
| CocoaAsyncSocket  | [github.com/robbiehanson/CocoaAsyncSocket](https://github.com/robbiehanson/CocoaAsyncSocket)         | 基于 Socket 的网络通信库          | BSD      | 支持      | 不支持 |

---

### 地图与导航

| 库名         | 官网                                  | 简介                         | 开源协议     | CocoaPods | SPM    |
| ------------ | ------------------------------------- | ---------------------------- | ------------ | --------- | ------ |
| BaiduMapKit  | [lbsyun.baidu.com](http://lbsyun.baidu.com)   | 百度地图 SDK               | 官方许可（非开源） | 支持      | 不支持 |
| BaiduNaviKit | [lbsyun.baidu.com](http://lbsyun.baidu.com)   | 百度导航与地图扩展 SDK       | 官方许可（非开源） | 支持      | 不支持 |
| BMKLocationKit | [lbsyun.baidu.com](http://lbsyun.baidu.com) | 百度定位及地理位置服务 SDK  | 官方许可（非开源） | 支持      | 不支持 |

---

### 测试辅助工具

| 库名             | 官网                                                                                   | 简介                                  | 开源协议 | CocoaPods | SPM    |
| ---------------- | -------------------------------------------------------------------------------------- | ------------------------------------- | -------- | --------- | ------ |
| OCMockito        | [github.com/jonkykong/OCMockito](https://github.com/jonkykong/OCMockito)               | Objective-C 模拟对象测试库              | MIT      | 支持      | 不支持 |
| OCHamcrest       | [github.com/hamcrest/OCHamcrest](https://github.com/hamcrest/OCHamcrest)               | 断言匹配库（测试用）                    | BSD      | 支持      | 不支持 |
| OCMock           | [github.com/erikdoe/ocmock](https://github.com/erikdoe/ocmock)                         | Objective-C 模拟框架                   | BSD      | 支持      | 不支持 |
| CoreBluetoothMock| 无公开官网                                                                            | 模拟 CoreBluetooth 功能的测试工具       | 未知     | 未知      | 未知   |
| OHHTTPStubs      | [github.com/AliSoftware/OHHTTPStubs](https://github.com/AliSoftware/OHHTTPStubs)         | HTTP 请求模拟（用于测试）                | MIT      | 支持      | 不支持 |
| Specta           | [github.com/specta/specta](https://github.com/specta/specta)                             | BDD 风格单元测试框架                    | MIT      | 支持      | 不支持 |
| Expecta          | [github.com/specta/expecta](https://github.com/specta/expecta)                           | 与 Specta 搭配使用的断言库              | MIT      | 支持      | 不支持 |

---

### 其他辅助工具

| 库名         | 官网                                                                                       | 简介                                | 开源协议 | CocoaPods | SPM    |
| ------------ | ------------------------------------------------------------------------------------------ | ----------------------------------- | -------- | --------- | ------ |
| SwiftPing    | [github.com/davejacobson/SwiftPing](https://github.com/davejacobson/SwiftPing)             | Swift 实现的 ICMP Ping 工具         | MIT      | 支持      | 未知   |
| SwiftGen     | [github.com/SwiftGen/SwiftGen](https://github.com/SwiftGen/SwiftGen)                        | 静态资源代码生成工具                | MIT      | 支持      | 支持  |
| WechatOpenSDK| [open.weixin.qq.com](https://open.weixin.qq.com)                                            | 微信开放平台 iOS SDK                | 官方许可   | 支持      | 不支持 |
| AlicloudPush | [alibabacloud.com](https://www.alibabacloud.com)                                            | 阿里云推送服务 iOS SDK              | 官方许可   | 支持      | 不支持 |
| PromiseKit   | [github.com/mxcl/PromiseKit](https://github.com/mxcl/PromiseKit)                           | 异步编程承诺（Promise）库            | MIT      | 支持      | 支持  |

---
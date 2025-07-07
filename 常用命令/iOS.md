# iOS开发

## 通过ipa、dSYM、crash日志等方式查看UUID

### 1、查看crash日志的构建UUID

①使用xcode连接崩溃设备，打开window->organizer，左侧应用列表选中你的app(DouBanJiang)，顶部tab切换到crash，找到你的crash，右键菜单show in finder->显示包内容->/DistributionInfos/all/Logs，即可看到当前类型的所有闪退列表。
②在终端执行以下命令。
        $ grep --after-context=2 "Binary Images:" DouBanJiang.crash
//注：这里，构建UUID是84966465-6F67-3AC5-88B5-B94DCF892F5E
，和路径应用程序的可执行文件是DouBanJiang.app/DouBanJiang。


### 2、查看.ipa包的UUID

①解压.ipa文件
 ②你在终端可以使用以下命令打印一个可执行的构建UUID
    $ xcrun dwarfdump --uuid  DouBanJiang.app/DouBanJiang


### 3、查看.dSYM文件的UUID

①使用终端输入以下命令即可
    $ dwarfdump --uuid  /Users/kimmac/Desktop/DouBanJiang.dSYM


查找symbolicatecrash

find /Applications/Xcode.app -name symbolicatecrash -type f

### 崩溃日志符号化

 ./symbolicatecrash + 你目录下的.crash路径 + 目录下app.dSYM文件路径 > 你要生成的文件名.crash

### 查看xx.app文件的uuid的方法：
dwarfdump --uuid xxx.app/xxx (xxx工程名)
### 查看xx.app.dSYM文件的uuid的方法令：
dwarfdump --uuid xxx.app.dSYM (xxx工程名)
### 查看xx.x 日志文件的uuid的方法令：
crash的uuid位于，crash日志中的Binary Images:中的第一行尖括号内。如：armv7<8bdeaf1a0b233ac199728c2a0ebb4165>

### 验证apple-app-site-association文件
curl -v  https://app-site-association.cdn-apple.com/a/v1/你的域名.com


### mobileprovision文件查看

security cms -D -i XXX.mobileprovision

## 项目配置

### 所有Supported Platforms
driverkit
macosx
iphoneos
iphonesimulator
appletvos
appletvsimulator
xros
xrsimulator
watchsimulator
watchos
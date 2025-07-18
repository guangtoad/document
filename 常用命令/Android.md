# Android 相关

## ADB辅助命令

### adb 截图

```
adb shell screencap -p /sdcard/02.png
```
### adb 截图并保存到电脑

```
adb exec-out screencap -p > screenshot.png
```

### adb 拉去图片
```
adb pull /sdcard/02.png
```

### 查看android cpu是32位还是64位

```
adb shell getprop ro.product.cpu.abi
```

## 性能监控

### 开启性能检测

```
adb shell setprop persist.traced.enable 1
```

### 冷启动性能检测
```
tools/record_android_trace  -t 10s -b 200mb gfx input view webview wm am sm audio video camera hal res dalvik rs bionic power pm ss database network adb vibrator aidl nnapi rro pdx sched irq i2c freq idle disk sync workq memreclaim regulators binder_driver binder_lock pagecache memory gfx ion
```

## APK 签名
```
jarsigner -verbose -keystore <#keystore路径#> -signedjar <#后签名APK输出路径#> <#未签名APK路径#> <#别名#>
```

## 查看CPU框架
```
adb shell getprop ro.product.cpu.abi
```

## Android 如何快速定位当前页面是哪个Activity or Fragment
(1)查看当前Activity ：```adb shell "dumpsys window w | grep name="```
(2)查看当前栈顶的Activity ：```adb shell dumpsys activity | grep "mFocusedActivity"```
(3)查看当前栈顶的Activity的Fragment ：```adb shell dumpsys activity your.package.name```
或者：
```adb shell dumpsys activity top```
查看帮助：```adb shell dumpsys activity -h```

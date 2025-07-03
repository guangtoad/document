# MacOS常用命令

## 1：禁用SafeSleep休眠模式——能节省出4GB-16GB空间

### 禁用SafeSleep功能，我们需要在终端中输入下面的命令：

```
sudo pmset -a hibernatemode 0
```

## 删除已经存在的sleepimage文件

```
sudo rm /private/var/vm/sleepimage
```

## 防止OS X继续创建该文件

```
touch sleepimage
chmod 000 /private/var/vm/sleepimage
```

## 2：移除系统嗓音文件——可以节省出500MB-3GB+硬盘空间
#所有嗓音文件删除

```
sudo rm -rf /System/Library/Speech/Voices/*
```
## 3：删除所有系统日志——可以节省出100MB-2GB硬盘空间
### 删除了系统日志

```
sudo rm -rf /private/var/log/*
```

## 4：删除快速查看生成的缓存文件——可以节省出100MB-300MB硬盘空间

```
sudo rm -rf /private/var/folders/
```

## 5：删除Emacs——可以节省出60MB+的硬盘空间

```
sudo rm -rf /usr/share/emacs/
```

## 6：删除临时文件——可以节省500MB-5GB硬盘空间

```
rm -rf /private/var/tmp/TM*
```

## 7：清除缓存文件——可以节省1GB-10GB硬盘空间
```
rm -rf ~/Library/Caches/*
```

## apachectl

### 环境配置
```
/private/etc
```

### 启动

```
sudo apachectl start 
```

### 配置测试

```
apachectl configtest
```

### 自动启动

```sudo launchctl unload -w /System/Library/LaunchDaemons/org.apache.httpd.plist```
如果哪天你想让它开机启动了,则将unload 改为 load:
```sudo launchctl load -w /System/Library/LaunchDaemons/org.apache.httpd.plist```


## 看端口
```
lsof -i :端口号
```

## 结束进程 
```
kill -9 pid
```

## 用法提示
#!/bin/bash
usage() {
    echo "用法: $0 [-a 参数A] [-b 参数B] [-c]"
    exit 1
}
## 初始化变量
```
param_a=""
param_b=""
flag_c=false
```

## 解析参数
```
while getopts ":a:b:c" opt; do
    case $opt in
    a)
        param_a="$OPTARG"
        ;;
    b)
        param_b="$OPTARG"
        ;;
    c)
        flag_c=true
        ;;
    \?)
        echo "无效选项: -$OPTARG" >&2
        usage
        ;;
    :)
        echo "选项 -$OPTARG 需要参数." >&2
        usage
        ;;
    esac
done

usage
```

## 显示隐藏文件

```
defaults write com.apple.finder AppleShowAllFiles -bool true
```

## 安装brew

```
/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
```

### 其他brew命令

brew list           列出已安装的软件
brew update     更新brew
brew home       用浏览器打开brew的官方网站
brew info         显示软件信息
brew deps        显示包依赖
## 删除brew

```
#/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/HomebrewUninstall.sh)
```

## 删除homebrew文件夹：

```
sudo rm -rf /usr/local/Homebrew
```

## 删除homebrew相关文件：

```
# sudo rm -rf /usr/local/Caskroom
# sudo rm -rf /usr/local/bin/brew
# sudo rm -rf /usr/local/share/doc/homebrew
# sudo rm -rf /usr/local/share/man/man1/brew.1
```


## 重启访达

```
killall Finder
```


## env 查看当前环境变量配置
（一）全局设置
下面的几个文件设置是全局的，修改时需要root权限
1）/etc/paths （全局建议修改这个文件 ）
编辑 paths，将环境变量添加到 paths文件中 ，一行一个路径
Hint：输入环境变量时，不用一个一个地输入，只要拖动文件夹到 Terminal 里就可以了。
2）/etc/profile （建议不修改这个文件 ）
全局（公有）配置，不管是哪个用户，登录时都会读取该文件。
3）/etc/bashrc （一般在这个文件中添加系统级环境变量）
全局（公有）配置，bash shell执行时，不管是何种方式，都会读取此文件。

### 环境变量文件

```
touch .bash_profile
```

### 使环境变量配置文件生效

```
source .bash_profile
```


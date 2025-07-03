# CentOS常用命令

## 关闭防火墙

```
sudo systemctl stop firewalld.service
```

## 永久关闭防火墙

```
sudo systemctl disable firewalld.service
```

## 查看防火墙状态

```
sudo systemctl status firewalld.service
```

## 启动SMB共享

```
systemctl restart smb
```

## 启动tomcat

```
/Application/apache-tomcat-9.0.65/bin/startup.sh
```
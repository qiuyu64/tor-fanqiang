# 简单3步 就可以用 TOR 翻墙

## 第一步 安装 Docker

Docker是一个通用的虚拟软件。一般可以在 [github](https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe)下载到。  [苹果系统下载](https://download.docker.com/mac/stable/Docker.dmg)

## 第二步 运行以下的命令
它的作用是运行一个TOR的服务在端口 9150

···
docker run -it -p 9050:9050 toronsynology/tor-client-minimal
···

## 第三步 配置使用 9150端口 进行网络连接

Window10 步骤 : 系统设置 -> 代理 -> 手动设置 -> 主机地址 输入127.0.0.1 -> 端口 输入 9150 -> 保存 即生效。

苹果系统 步骤 ：系统设置 -> 网络 -> 高级 -> 代理标签 -> SOCK 代理 -> 127.0.0.1 ： 9150


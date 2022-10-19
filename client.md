## 客户端安装教程

客户端安装教程非常简单

1. 把McVersioningClient.jar复制到你即将要发布给玩家的服务器客户端文件夹里，放在启动器旁边也就是.minecraft目录的旁边
2. 用压缩软件打开McVersioningClient.jar，把config.yml文件解压到McVersioningClient.jar的旁边，打开config.yml文件进行编辑
3. 将刚刚服务端程序输出的API地址粘贴到config.yml中的server选项后面，然后保存关闭
4. 双击运行McVersioningClient.jar，如果一切正常，就会开始更新第一个版本，更新完成后客户端的版本号会保存在mv-version.txt里面，默认放在程序旁边

### 一键启动

一键启动可以在Minecraft游戏启动时候同时更新游戏文件，可以和启动器做到无缝集成式更新，正式环境中非常建议使用一键启动来更新

一键启动目前支持两个平台：

+ [Windows平台](javaagent-windows.md)
+ [Android平台](javaagent-android.md)
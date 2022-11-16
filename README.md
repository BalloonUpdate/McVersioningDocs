## Mc Versioning Docs

!> Mc Versioning系列有文件漏更新的严重bug，请勿再使用。若已使用，请尽快更换为其它版本系列

Mc Versioning 是一个简单易上手的Minecraft服务器客户端更新程序，没有难以理解的头疼概念，也没有混乱复杂的文件结构。软件以简单可靠为设计目标，大大降低了小白的使用门槛

软件是一个服务端——客户端架构的独立应用程序，并非模组或者资源包或插件。

在使用软件之前，如果你有开服相关的经验或者搭建网站经验，那么对使用Mc Versioning软件将会非常有帮助

软件的优点：

1. **检测文件速度快**：基于版本号的更新速度更快。磁盘IO开销更小，对移动端设备更加友好
2. **智能检测变动文件**：发布新版本时Mc Versioning会自动检测到哪些文件改变，并自动生成差异记录
3. **不删玩家的模组文件**：使用Mc Versioning玩家可以自由添加自己的mod而不用担心被误更新删除

## 安装教程

> Mc Versioning是个易上手的软件，所以不会有难以理解的安装步骤

安装之前，有些事情你要知道：Mc Versioning有3个可执行文件，其中两个是给服务端用的，另外一个是给客户端用的

1. McVersioning.jar：服务端软件，用来管理和打出新的版本包
2. MiniHttpServer.jar：服务端软件：用来开启一个HttpServer供客户端下载
3. McVersioningClient.jar：客户端软件，用来更新客户端文件

教程目录：

+ [服务端安装教程（v0.1）](server.md)
+ [服务端安装教程（v0.0）](server-v0.0.md)
+ [客户端安装教程](client.md)
+ [静态工具教程](static-server.md)
+ [常见问题解答（有技术门槛要求）](faq.md)
+ [public目录下的文件用途说明](public-files-illustration.md)
+ [Windows平台一键启动教程](javaagent-windows.md)
+ [Android平台一键启动教程](javaagent-android.md)




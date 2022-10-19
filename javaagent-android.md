## Android平台一键启动

教程这里以澪作为示例，其它启动器大同小异。其它启动器的教程会慢慢更新

1. 首先确保McVersioningClient在电脑上双击启动没问题
2. 将McVersioningClient文件和配置文件（如果有）一起复制到`/sdcard/MioLauncher/xxx.jar`目录下（`xxx`是McVersioningClient的实际文件名）
3. 打开澪，切换到`游戏配置`页面，在游戏参数的最前面插入一段JVM参数`-javaagent:/sdcard/MioLauncher/xxx.jar`（`xxx`换成McVersioningClient的实际的文件名）
4. 点击保存按钮，然后重启澪
5. 启动游戏测试效果。如果你要看McVersioningClient的工作过程，可以打开澪的日志窗口

## 性能说明

Android平台通常使用ARM处理器。ARM的性能没有x86那么强劲，所以请尽量控制每次客户端体积大小

虽然McVersioning现在在性能方面已经没有了短板，但在使用的过程中还是尽量控制一下更新量的大小。较小的更新量不仅能节省服务器流量，还能加快游戏的启动速度

## 游戏闪退崩溃

虽然McVersioning可以跑在Android平台上，但是却无法像PC端那样显示更新进度条窗口，一切的更新过程都是在后台进行的

所以当McVersioningClient在运行过程中遇到网络问题，或者其它错误时，会主动崩溃掉Minecraft进程！！！这是刻意的设计，不要一看到游戏崩了就开始各种问候家人

如果启动过程中发生闪退或者崩溃，请首先翻阅日志末尾，判断是否是McVersioningClient主动使得Minecraft进程崩溃的，还是说是其它原因

如果是McVersioningClient主动崩溃，错误信息中会有中文文字很清晰地说明具体是什么原因导致的游戏崩溃。并且每条日志前面都会有`McVersioning`的字样标明这是一条McVersioning的消息。如果找不到McVersioning相关的字样说明是其它原因导致的崩溃，也就是说崩溃和McVersioning没有直接的关系

如果你不喜欢这种直接崩溃的做法，可以在配置文件里设置`no-throwing`选项来让McVersioningClient遇到错误时不打断游戏启动的过程，而不是直接把游戏给崩了

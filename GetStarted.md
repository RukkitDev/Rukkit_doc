# 引言
设置一个 Rukkit 服务器简单而轻松（至少现在如此），跟随下列教程，你就可以拥有一个属于自己的铁锈战争服务器。

# 设置 Java 环境
从 Oracle 官网或者其他正规渠道下载 Rukkit 所需的 Java 环境（又称 JRE）

[清华大学镜像站提供的 JDK17](https://mirrors.tuna.tsinghua.edu.cn/Adoptium/17/jdk/x64/windows/)

安装时请勾选安装到 PATH，方便在控制台直接使用.此处笔者使用 Win 11 作为演示系统。启动终端，输入 ```java -version``` 回车，出现以下类似的内容即安装成功
```bash
openjdk version "17.0.7" 2023-04-18 LTS
OpenJDK Runtime Environment Microsoft-7626293 (build 17.0.7+7-LTS)
OpenJDK 64-Bit Server VM Microsoft-7626293 (build 17.0.7+7-LTS, mixed mode, sharing)
```

# 从 release 下载 Rukkit 程序并执行

[Release页面](https://github.com/RukkitDev/Rukkit/releases)

从 release 页面下载最新版本的 Rukkit zip文件，解压到单独的目录，双击start.bat启动服务端，当看到如下信息时说明启动成功：

```
[XXX-XX-XX XX:XX:XX INFO] [GameServer]: Done! (369ms)
```

此时 Rukkit 已经在 5123 端口上成功运行，您可以启动游戏尝试连接服务器。

# 如何将我的服务器发布到列表？

要将你的服务器发布到官方列表，你需要一台拥有公网IP的服务器，和 [本插件](https://github.com/RukkitDev/example-uplist-plugin)。由于特殊原因，该插件不提供成品，请您自行编译安装。

如果没有公网IP，你的服务器就不能发布到官方列表上，但可以使用 frp 等端口转发服务来进行远程联机，
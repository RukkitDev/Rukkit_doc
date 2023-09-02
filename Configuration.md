# 引言
此处讲解目前 Rukkit 配置文件内各选项的作用，之后可能会整合入 Rukkit 项目中提供示例 rukkit.yml。

# 配置文件

```yml
# snakeyml 自动生成的 Java 类信息 
!!cn.rukkit.config.RukkitConfig

# 服务器的 UUID，自动生成
UUID: 00000000-0000-0000-0000-000000000000

# 配置文件名称
configName: rukkit.yml

# 是否处在 debug 模式下，用于插件开发或调试
isDebug: true

# 语言选项，影响到控制台输出和游戏内服务器输出语言
lang: zh_CN

# 日志位置，废弃内容
logPath: rukkit.log

# 数据包最大字节数，大于该大小的数据包会被舍弃
maxPacketFrame: 8192

# 房间内最大玩家数(1-100)
maxPlayer: 10

# 最大房间数
maxRoom: 5

# 开始一场对局最小所需的玩家数
minStartPlayer: 4

# 在线模式，用于对涉及官方列表插件的限制，日后可能会被移除
onlineMode: false

# 玩家掉线阈值(ms)，在规定时间内未返回 ping 包的玩家会被强制断线
pingTimeout: 8000

# 注册时间延迟(s), 在规定时间内未向服务器发送玩家信息的客户端会被强制断线
registerTimeout: 5

# 服务器 MOTD，即服务器名称
serverMotd: My Rukkit server

# 服务器监听端口
serverPort: 5123

# 服务器用户名
serverUser: RUKKIT

# 单人模式：启用此选项时服务器不会因为游戏中只剩下一位玩家而强制终止对局
singlePlayerMode: false

# 启用断线重连（同步）
syncEnabled: true

# 线程池大小，增大也许会提升性能？
threadPoolCount: 8

# 使用顺序执行模式：该模式使服务器使用原版的游戏指令处理模式，提升稳定性但是会增加操作延迟
useCommandQuere: false

# 欢迎信息：玩家进入服务器服务器所发送的欢迎消息，目前版本没有 format
welcomeMsg: Welcome to Rukkit server, {user}!

```
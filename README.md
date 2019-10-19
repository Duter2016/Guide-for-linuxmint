# Guide-for-linuxmint
Linux Mint 18.3+（含19.2） 双系统安装及优化指导手册
### 更新时间：2019.09.21

## 文档更新说明
见文章[《Linux Mint 18.3+（含19.2） 双系统安装及优化指导手册》](https://duter2016.github.io/2019/09/15/LinuxMint18.3+-%E5%90%AB19.2-%E5%8F%8C%E7%B3%BB%E7%BB%9F%E5%AE%89%E8%A3%85%E5%8F%8A%E4%BC%98%E5%8C%96%E6%8C%87%E5%AF%BC%E6%89%8B%E5%86%8C/)

## 目录	
```
说明......................................................................................................................................................1
一、 Linuxmint 及 Windows 双系统安装.........................................................................................1
1.1 EasyBCD 安装系统准备（ 基于 BIOS 启动方式） .........................................................1
1.2 系统安装过程.......................................................................................................................2
1.3 在 windows 下修复 LinuxMint 开机启动项...................................................................... 7
1.4 基于 UEFI 启动方式下安装 Linuxmint 和 windows 双系统............................................9
1.5 关于双系统下， linuxmint 环境中有时对对挂载的 NTFS 磁盘分区无写权限的问题...9
二、 Linuxmint 系统优化设置及软件安装...................................................................................... 11
2.1 Linuxmint 系统优化............................................................................................................ 11
2.1.1 替换国内软件源...................................................................................................... 11
2.1.2 更新系统.................................................................................................................. 11
2.1.3 安装 Wicd 网络管理器............................................................................................11
2.1.4 添加 windows 字体及关于 Freetype 渲染的问题..................................................13
2.1.5 安装系统缺失的部分汉化语言包...........................................................................16
2.1.6 安装输入法..............................................................................................................17
2.1.7 更新系统驱动...........................................................................................................19
2.1.8 更换系统主题...........................................................................................................19
2.1.9 轻松搞定 Linux+Win 双系统时间差异...................................................................22
2.1.10 修复系统托盘上的日期格式.................................................................................23
2.1.11 插入鼠标后停用 touchpad 功能............................................................................23
2.1.12 Thinkpad 笔记本安装电源管理模块.....................................................................24
2.2.13 使用 thinkfan 控制 thinkpad 风扇转速..................................................................37
2.1.14 Thinkpad 笔记本安装硬盘保护模块.....................................................................42
2.1.15 使用 ppa 镜像代理加速服务................................................................................ 43
2.2 安装非系统类软件.............................................................................................................45
2.2.1 安装 Flash Player...................................................................................................... 45
2.2.2 安装多媒体解码.......................................................................................................45
2.2.3 安装 rar 和其它归档工具.........................................................................................45
2.2.4 安装剪贴板管理器...................................................................................................45
2.2.5 安装 Guake 下拉终端...............................................................................................46
2.2.6 安装 Uget 及 Aria2 下载管理器.............................................................................. 46
2.2.7 安装 Deluge BitTorrent 客户端................................................................................47
2.2.8 安装 Hardinfo - 系统信息工具............................................................................... 47
2.2.9 安装 Conky............................................................................................................... 47
LinuxMint 18.3+ 系统安装及优化指导手册
2
2.2.10 Linux 快速安装 firefox esr...................................................................................48
2.2.11 安装 wine 和 playonlinux 及 Deepin-wine 方案...................................................48
2.2.12 Linux 系统安装 wineQQ........................................................................................50
2.2.13 解决 Rhythmbox 中文乱码问题........................................................................... 50
2.2.14 Fcitx 输入法无法输入中文， 光标不跟随的 applicaiton： .................................51
2.2.15 解决 Fcitx 中文输入法无法输入全角中括号【 】 ..............................................51
2.2.16 添加 Fcitx 中文拼音版常用表情符号和带圈数字..............................................51
2.2.17 启用 Fcitx 英文输入法的英文单词自动补全功能..............................................53
2.2.18 Fcitx-rime 中州韵安装及自然码、 小鹤双拼、 小鹤音形配置........................... 54
2.2.19 安装 sublime text 3(不使用这个软件了)..............................................................67
2.2.20 安装 Pycharm（ 社区版） 编辑器.........................................................................68
2.2.21 Python 安装第三方模块（ pip3） ..........................................................................69
2.2.22 Stardict 和 GoldenDict， 及离线字典的安装........................................................70
2.2.23 Linux 和 Mac 下的微信电脑版 electronic-wechat(非官方)................................. 71
2.2.24 安装 shadowsocks-qt5 或 electron-ssr 或 Goflyway............................................74
2.2.25 Xfce 终端 xfce4-terminal -可以放背景图片......................................................... 78
2.2.26 安装 Psensor 温度感应器......................................................................................78
2.2.27 安装 flux 护眼软件................................................................................................78
2.2.28 安装 Moon Player 播放器.................................................................................... 79
2.2.29 安装 Foxit 阅读器..................................................................................................79
2.2.30 安装阿里旺旺........................................................................................................79
2.2.31 屏幕截图工具 Shutter 和 Flameshot.....................................................................81
2.2.32 安装屏幕录像软件 RecordMyDesktop 和 Kazam、 Peek....................................82
2.2.33 安装 Java 运行环境...............................................................................................84
2.2.34 股票管理软件 JStock............................................................................................ 86
2.2.35 安装可输入中文的 Telegram 客户端...................................................................88
2.2.36 鼠标模拟点击器 Actiona...................................................................................... 89
2.2.37 图片压缩工具 Trimage..........................................................................................89
2.2.38 视频编辑器 Openshot............................................................................................89
2.2.39 安装 OpenCV.........................................................................................................90
2.2.40 百度云下载工具 proxyee-down 及官方版...........................................................90
2.2.41 安装 Xmind 8 或 Xmind Zen（ 二选一即可） .....................................................91
2.2.42 极简流量悬浮窗工具 Flow 和 Minimalist........................................................... 93
2.2.43 安装罗技鼠标驱动................................................................................................94
2.2.44 安装 UI 版定时任务工具 Crontab........................................................................94
2.2.45 桌面快件方式（ .desktop） 文件创建工具...........................................................94
2.2.46 网易云音乐播放器................................................................................................95
2.2.47 Thunderbird 推荐使用的几个扩展程序............................................................. 97
LinuxMint 18.3+ 系统安装及优化指导手册
3
2.2.48 给 IRC 通信软件 Hexchat 配置脚本....................................................................97
2.2.49 Epson 爱普生针式打印机 LQ-630KII 驱动安装..................................................98
2.2.50 集本地与云笔记于一体的 GitNote 笔记软件..................................................... 99
2.2.51 杀毒软件 clamTK 使用 http 代理更新病毒库的方法.......................................102
更多应用程序： ..............................................................................................................104
```

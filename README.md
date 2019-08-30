# Guide-for-linuxmint
Linux Mint 18.3+（含19.2） 双系统安装及优化指导手册
### 更新时间：2019.08.30
## 目录	
说明	1
一、 Linuxmint及Windows双系统安装	1
1.1  EasyBCD安装系统准备（基于BIOS启动方式）	1
1.2 系统安装过程	2
1.3 在windows下修复LinuxMint 开机启动项	7
1.4 基于UEFI启动方式下安装Linuxmint 和windows双系统	9
1.5 关于双系统下，linuxmint环境中有时对对挂载的NTFS磁盘分区无写权限的问题	9
二、Linuxmint系统优化设置及软件安装	11
2.1 Linuxmint系统优化	11
2.1.1 替换国内软件源	11
2.1.2 更新系统	11
2.1.3 安装Wicd网络管理器	11
2.1.4 添加windows字体及关于Freetype渲染的问题	13
2.1.5安装系统缺失的部分汉化语言包	16
2.1.6 安装输入法	17
2.1.7更新系统驱动	19
2.1.8更换系统主题	19
2.1.9轻松搞定Linux+Win双系统时间差异	22
2.1.10修复系统托盘上的日期格式	23
2.1.11 插入鼠标后停用touchpad功能	23
2.1.12 Thinkpad笔记本安装电源管理模块	24
2.2.13使用thinkfan控制thinkpad风扇转速	37
2.1.14 Thinkpad笔记本安装硬盘保护模块	42
2.2 安装非系统类软件	43
2.2.1安装Flash Player	43
2.2.2安装多媒体解码	44
2.2.3安装rar和其它归档工具	44
2.2.4安装剪贴板管理器	44
2.2.5安装Guake下拉终端	44
2.2.6安装Uget及Aria2下载管理器	45
2.2.7安装Deluge BitTorrent客户端	46
2.2.8安装Hardinfo - 系统信息工具	46
2.2.9安装Conky	46
2.2.10 Linux 快速安装 firefox esr	47
2.2.11 安装wine和playonlinux及Deepin-wine方案	47
2.2.12 Linux系统安装wineQQ	49
2.2.13 解决Rhythmbox中文乱码问题	49
2.2.14 Fcitx输入法无法输入中文，光标不跟随的applicaiton：	50
2.2.15 解决Fcitx中文输入法无法输入全角中括号【】	50
2.2.16 添加Fcitx中文拼音版常用表情符号和带圈数字	50
2.2.17 Fcitx-rime中州韵安装及自然码、小鹤双拼配置	52
2.2.18 安装sublime text 3(不使用这个软件了)	65
2.2.19 安装Pycharm（社区版）编辑器	66
2.2.20 Python安装第三方模块（pip3）	67
2.2.21 Stardict和GoldenDict，及离线字典的安装	67
2.2.22 Linux和Mac下的微信电脑版electronic-wechat(非官方)	68
2.2.23 安装 shadowsocks-qt5或electron-ssr	71
2.2.24 Xfce终端xfce4-terminal -可以放背景图片	74
2.2.25 安装Psensor温度感应器	74
2.2.26 安装flux护眼软件	74
2.2.27 安装Moon Player 播放器	75
2.2.28 安装Foxit阅读器	75
2.2.29 安装阿里旺旺	76
2.2.30 屏幕截图工具Shutter和Flameshot	78
2.2.31 安装屏幕录像软件RecordMyDesktop和Kazam、Peek	79
2.2.32 安装Java运行环境	80
2.2.33 股票管理软件JStock	82
2.2.34 安装可输入中文的Telegram客户端	84
2.2.35 鼠标模拟点击器Actiona	85
2.2.36 图片压缩工具Trimage	85
2.2.37 视频编辑器Openshot	85
2.2.38 安装OpenCV	86
2.2.39 百度云下载工具proxyee-down及官方版	87
2.2.40 安装Xmind 8或Xmind Zen（二选一即可）	87
2.2.41 极简流量悬浮窗工具Flow和Minimalist	89
2.2.42 安装罗技鼠标驱动	90
2.2.43 安装UI版定时任务工具Crontab	90
2.2.44 桌面快件方式（.desktop）文件创建工具	91
2.2.45 网易云音乐播放器	91
2.2.46  Thunderbird推荐使用的几个扩展程序	93
2.2.47 给IRC通信软件Hexchat配置脚本	93
2.2.48 Epson爱普生针式打印机LQ-630KII驱动安装	94
2.2.49 集本地与云笔记于一体的GitNote笔记软件	95
2.2.50 杀毒软件clamTK使用http代理更新病毒库的方法	98
更多应用程序：	100

# budgetKvm

鉴于全国越演越烈的疫情，导致很多人被关在家里，觉到很有必要搞一个硬件版本的远程桌面方案，做到真远程办公。

不同于成熟的方案，这个方案提供的是思路与实现方式。

方案一:

第一 硬件材料准备
* X96 MAX+ 一台（淘宝二手200来快）
* USB HDMI 视频采集卡一张 (京东上80来块，只着重于实现，不考虑啥高清呀，4k的）

第二 软件准备
* 编译X96 MAX+ 的openwrt 固件
* 配置openwrt支持usb_gadget的支持，给电脑提供USB鼠标键盘的支持（当然给PC提供网卡，还有U盘也是可以支持的）
* 视频采集卡的驱动配置。
* 编译X96 MAX+的远程访问软件，比如frp， UDP穿透，DDNS等。
* 为了显示可以将视频跟鼠标键盘转换成VNC供远程使用。

第三 安装
* 刷入固件，并且将X96 MAX+的OTG口连接电脑。
* 视频采集卡，USB口接X96 MAX+， HDMI端接电脑的视频输出。

备选方案
android 手机一台，可以自行编译kernel的那种，比如nexus,Tanix TX3 Mini, MINIX NEO U22-XJ,X96 Tanix TX3

最后总结：你值得拥有，适合一下使用场景（不限于）：
* 远程办公，安装操作系统
* 游戏自动话脚本，防止游戏作弊检测。
* 临时给没接显示器的设备当做临时显示器使用。

# 参考链接
[编译一](https://github.com/ylqjgm/mknop)
[编译二](https://github.com/ophub/amlogic-s9xxx-openwrt)
[刷版本](https://www.right.com.cn/forum/thread-4035964-1-1.html)
[tightvnc](https://github.com/TurboVNC/tightvnc/wiki)
[ultravnc](https://github.com/ultravnc/UltraVNC)

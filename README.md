# 这是一个笔记本，用来记录Linux桌面版日常家用笔记

![](https://github.com/redomCL/Linux-desktop-note/blob/main/Ubuntu.png)
![](https://github.com/redomCL/Linux-desktop-note/blob/main/duckstation.png)
![](https://github.com/redomCL/Linux-desktop-note/blob/main/gnome-software.png)
![](https://github.com/redomCL/Linux-desktop-note/blob/main/synaptic.png)

# 前言：
* Linux目前的发展相比Windows真的不适合日常家用娱乐，易用性要差的相当多，但是为了不完全依赖商业形式运转的Windows操作系统，我还是尽可能的去了解一下Linux，本合集为Linux为了日常家用娱乐为主的笔记。 具体主要用途：
*  1、家庭影音：主要以跨平台的优秀播放器mpv为主，也可以用基于mpv的gnome mpv、smplayer
*  2、网络通讯：微信、QQ、跨平台的优秀浏览器firefox
*  3、游   戏：steam和wine，Linux原生模拟器
*  ...

## 一、包管理相关：软件安装
* 实际上GNOME除了作为Ubuntu的桌面，同时也为大部分包管理器（软件商店）提供了一个图形界面，apt、snap、flatpak和dnf都可以用gnome-software作为图形包管理器（图形软件商店）

* Deb/Ubuntu .deb：Ubuntu；前端包管理器apt，图形前端包管理器synaptic/gnome-software，安装软件的基础。

* Ubuntu snap：Ubuntu；前端包管理器snap，有图形前端snap-store/gnome-software，用于对apt的扩充。

* Fodera/RedHat .RPM：Fodera；RedHat；前端包管理器dnf，图形前端包管理器gnome-software。

* openSUSE：YaST/YaST2图形前端包管理器。

* *fuse：用户空间文件系统，用于对apt的扩充，ubuntu下通过apt安装libfuse2，实现对appimage独立包的直接运行。

* * *Flatpak：多种Linux桌面发行版；前端包管理器flatpak，图形前端包管理器gnome-software，用于对apt的扩充。包含大量游戏模拟器软件。

## 二、Linux显卡驱动篇

### AMD显卡篇

* 目前仍在探索阶段，暂且总结一下自己认知下的情形：

* 1、首先是AMD官方自己为Linux制作的fglrx系列：这是闭源的，也正因为如此，所以并不能随着Linux各发行版的更新直接安装，会逐渐出现不兼容。当AMD官方停止更新后，那么这块显卡在更新的Linux发行版上也就随之丧失了这款驱动。

* 2、mesa3D驱动：这是一款在Linux上支持不仅限于AMD的各种显卡驱动，可以支持OGL、VLK等API，更新很及时，如果显卡在后期不再受官方的支持，我想可能这是最好的选择了。

* 3、AMDVLK开源驱动：AMD的开源驱动项目，貌似可以更持久的维护显卡，不过支支持RX400及以上的显卡，更老的显卡没有办法使用

* 另外还有一款叫做corectrl的工具可以充当AMD显卡的图形控制面板，风格类似于AMD的深红/肾上腺素UI

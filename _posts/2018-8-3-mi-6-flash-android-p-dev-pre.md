---

layout:     post

title:      小米6刷 Android P

subtitle:   小米6刷入Android P DP5 实战记录

date:       2018-8-3

author:     csc0330

header-img: img/2018-1.jpg

catalog: true

tags:

    - Android

---
[在本站全球版查看 Global version][1]
## 刷入Recovery ##
这里是先获取的MIUI Root权限，需要打开系统安全中心，开启Root权限。具体方式在此不列出请自行查询。
获取Root后从酷安网下载TWRP的app（包名：me.twrp.twrpapp），用于刷入Recovery。选择合适的Recovery刷入。当然，adb也行，具体使用那种方式取决于你的习惯。
**需要特别注意的是必须使用支持PT的Recovery。**
Recovery：`https://sagit.sbwml.net/?dir=tools/Recovery-treble`

## 备份 ##
有备无患。
请自行备份所有文件，因为在接下来步骤需要清除 **所有文件** ！
**特别提醒：本文只作引导，由于操作失误等造成的任何问题及责任本站不负。刷机有风险请谨慎考虑！**

## 下载必要的文件 ##
请下载必要的文件：
1. Android P的ROM包：`https://sagit.sbwml.net/?dir=Android_P`
2. 解决发热问题的第三方内核：`https://share.weiyun.com/5Z7LYXH`
3. 解决基带问题的底包：`https://sagit.sbwml.net/tools/Firmware-sagit/miui_MI6Global_V9.5.6.0.OCAMIFA_Firmware.zip`
4. （可选）Magisk安装及卸载包：`https://sagit.sbwml.net/?dir=tools/Magisk-v16.6`

## 刷入系统 ##
请确保使用支持 Treble 的 TWRP Recovery.
1. 清除 cache, data, system, vendor, storage 分区.
2. 复制Android P 刷机包到内置存储.如果不能复制，请把ROM复制到adb所在的文件夹或者任意文件夹（取决于你是否安装了adb），使用`adb push rom.zip sdcard/`来推入ROM。
3. 安装Android P zip刷机文件.
4. 格式化data.（如果不格式，刷机包会一直保存在隐藏路径中.）
5. 重启系统

## 刷入GPU驱动、内核、底包 ##
1. 进入TWRP；
2. 分别安装上述内容并重启。

## 开始使用 ##
到此，若没有出现问题你将进入Android P。
[1]:http://global.scchan.com/2018/08/18-8-36android-p.html

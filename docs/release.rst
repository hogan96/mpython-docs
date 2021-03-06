.. _release:

固件发布
========

mpython_v2.0.1
------------------

===============  ====================================
 **发布日期**：    2020/01/13
 **固件下载**:     :download:`mpython_firmware_v2.0.1 <https://github.com/labplus-cn/mpython/releases/download/v2.0.1/mpython_v2.0.1.bin>`
===============  ====================================

**日志**：

* 修正有时出现不能录音BUG
* 加入指南针校正功能
* urequests修改ssl为默认不握手
* 增加字体显示函数
* 增加logging模块
* 更新天气图标模块
* 修改一些已知小BUG

mpython_v2.0.0
------------------

===============  ====================================
 **发布日期**：    2019/12/25
 **固件下载**:     :download:`mpython_firmware_v2.0.0 <https://github.com/labplus-cn/mpython/releases/download/v2.0.0/mpython_v2.0.0.bin>`
===============  ====================================

**日志**：

* 升级micropython，IDF升级到v4.0
* 重新构建项目框架
* 加入蓝牙ble
* 加入录音功能
* 加入磁力计
* 硬件修改了usb接口，按键
* urequest模块,增加POST表单功能
* oled.DispChar()增加返回字符宽度参数
* 增加urllib.parse模块(URL解析)

mpython_v1.5.1
------------------

===============  ====================================
 **发布日期**：    2019/9/25
 **固件下载**:     :download:`mpython_firmware_v1.5.1 </../firmware/mpython_firmware_v1.5.1.bin>`
===============  ====================================

**日志**：

* `music` 模块添加5首中文歌曲:

   * GE_CHANG_ZU_GUO（歌唱祖国）
   * DONG_FANG_HONG（东方红）
   * CAI_YUN_ZHUI_YUE（彩云追月）
   * ZOU_JIN_XIN_SHI_DAI（走进新时代）
   * MO_LI_HUA（茉莉花）
   * YI_MENG_SHAN_XIAO_DIAO(沂蒙山小调)

* 修正舵机、马达共用一个LED PWM高速通道相互干扰问题。
* 修正已知Bug


mpython_v1.5.0
-----------------

===============  ====================================
 **发布日期**：    2019/7/22
 **固件下载**:     :download:`mpython_firmware_1.5.0-23 </../firmware/mpython_firmware_v1.5.0-23.bin>`
===============  ====================================

**日志**：

* 固件合并字库,烧录固件起始地址0x00;
* 文件系统空间由1M扩大至2M(字库起始地址由为0x300000改为0x400000);
* 增加 `gui.Image` 类支持1bit bmp、pbm图片格式;
* 增加 `gui.UI.qr_code` 二维码显示;
* 增加灯带 `NeoPixel.brightness` 亮度调整函数
* 增加 `sdcard` 模块;
* `request` 增加file参数,支持文件上传;
* `audio` 模块增加录音功能;
* C层实现绘图函数,提升效率;
* 内置bluebit,parrot.py等;
* 修正已知Bug;



mpython_v1.4.0
------------

===============  ====================================
 **发布日期**：    2019/4/22
 **固件下载**:     :download:`mpython_firmware_1.4.0 </../firmware/mpython_firmware_1.4.0.zip>`
===============  ====================================

**日志**：

* 增加 ``radio`` 无线模块,支持无线广播功能；
* 增加当捕抓到KeyboardInterrupt中断或退出main循环,会关闭Timer和Thread；
* 修改music已知Bug；


mpython_v1.3.0
------------

===============  ====================================  
 **发布日期**：    2019/4/8
 **固件下载**:     :download:`mpython_firmware_1.3.0 </../firmware/mpython_firmware_1.3.0.zip>`
===============  ====================================

**日志**：

* 增加 ``audio`` 模块,支持掌控板音频播放功能和TTS文字转语音功能；
* 修正 ntptime.py 时区错误的bug;


mpython_v1.2.0
------------

===============  ====================================  
 **发布日期**：    2019/1/29
 **固件下载**:     :download:`mpython_firmware_1.2.0 </../firmware/mpython_firmware_1.2.0.zip>`
===============  ====================================

**日志**：

* mpython库内置到固件,文件系统不需要刷入了;
* 修改开机动画,变为静态画面,不占用开机时间;
* 修改代码错误提示页面,可详细指示错误位置和详细信息,keyboardinterrupt不再出现错误提示
* 修复i2c的读取blue:bit模块的一些问题;
* 增强内置传感器读取稳定性,错误后重试5次才报错;

mpython_v1.1.1
--------------

===============  ====================================  
 **发布日期**：      
 **固件下载**:     :download:`mpython_firmware_1.1.1 </../firmware/mpython_firmware_1.1.1.zip>`
===============  ====================================

**日志**：

* 固件烧录起始地址由0x1000改为0x00
* 修改开机启动动画时间为0.5S
* 修改urequest的一些错误
* 修改ntptime的服务器地址,并提供用户指定地址接口
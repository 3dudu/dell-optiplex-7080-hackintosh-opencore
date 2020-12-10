# Dell-optiplex-7080MFF-hackintosh-opencore

### 硬件

处理器：Intel Core i7-10700t

芯片组：Intel Q470

内存：16G DDR4 2666 * 2

显卡：UHD630

声卡：ALC256 (内置扬声器+耳麦一体+音频输出)

网卡：Intel I219-LM7

扩展卡：dell type-c alt（dp+usb3.0）

无线网卡：BCM943602CS with NGFF Adapter

![屏蔽 11，12 针脚](https://github.com/3dudu/dell-optiplex-7080-hackintosh-opencore/blob/main/1605583200393.jpg?raw=true)

> 转接卡需要屏蔽 11，12 针脚，否则连上wifi很快就会死机。



硬盘1：KIOXIA-EXCERIA SSD 512G

硬盘2：NVMe KIOXIA 256GB 

硬盘3：KING SHARE M300064G

### 正常工作：

1.变频 HWP

2.显卡、网卡、声卡、无线网卡、蓝牙

3.睡眠

4.修改有线网卡驱动，支持网络唤醒开机 [https://github.com/3dudu/IntelMausi]

5.软重启

> 已解决，ACPI补丁可以修正！

### 不正常工作：

1. ~~不能重启~~

2.DP不能输出声音

> 当接两台显示器时，DP声音可以输出。本人另一台显示器是typre-c转HDMI接入

3.插入耳机，声音输出不能自动切换，需要重开机。

> 当接两台显示器时，耳机声音可以切换。本人另一台显示器是typre-c转HDMI接入。耳麦一体还不可以

### BIOS设置
|设置项|值|
|----|---|
|SATA Operation | AHCI |
|Integrated NIC | Enabled |
|Secure Boot Enable | unChecked |
|Secure Boot Mode | Audit Mode |
|SGX | Disabled |
|SpeedStep | Enable |
|C-States Control | Checked |
|Turboost | Enable |
|HyperThread Control | Enable |
|Intel Speed Shift Technology | Enable |
|Deep Sleep Control | Disabled |
|USB Wake Support | unChecked |
|Wake on LAN/WLAN | Lan only |
|Block Sleep | unChecked |
|Fastboot | Minimal |
|Virtualization | Enable |
|VT For Direct I/O | unChecked |
|ASPM | Auto |

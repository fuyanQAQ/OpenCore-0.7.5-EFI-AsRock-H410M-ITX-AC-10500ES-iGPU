# OpenCore-0.7.5-EFI-AsRock-H410M-ITX-AC-10500ES-iGPU
# macOS Big Sur  and macOS Monterey
# Hackintosh

## 配置

| Items       | Model               |
| ----------- | ------------------- |
| Motherboard | AsRock H410M-ITX/AC |
| CPU         | Intel Core i5-10500ES |
| RAM         |  8GB DDR4 2666 MHz |
| Hard Disk   | 杂盘        |
| GPU         | UHD 630             |
| Sound Card  | Realtek ALC887      |
| Ethernet    | (Onboard)           |
| WLAN        | Intel Dual Band Wireless-AC 3168 |

## 功能
- [x] 板载声卡
- [x] 板载网卡
- [x] 核显硬解
- [x] wifi/蓝牙([大神的intel网卡驱动](https://docs.oiw.workers.dev/itlwm/))(已删除驱动需要自己添加因为不知道你们需要大乌苏还是蒙特雷)
- [x] 睡眠 / 唤醒
- [x] USB2.0 / USB 3.0
- [x] DRM
- [x] 核显dp/hdmi输出



## BIOS设置选项列表
# 禁⽤清单
| 名称        | 说明               |
| ----------- | ------------------- |
| Fast Boot   | 快速启动 |
| VT-d        | (can be enabled if you set DisableIoMapper to YES) - VT-d（如果DisableIOMapper Quicks设置为YES，则可以启⽤） |
| CSM         | 兼容性⽀持模块 |
| Thunderbolt   | 雷雳        |
| Intel SGX         | 英特尔SGX             |
| Intel Platform Trust  | 英特尔平台信任      |
| CFG Lock (MSR 0xE2 write protection)    | CFG锁（MSR 0xE2写保护）（必须关闭，如果找不到该选项，则在OpenCore的config-内核-> Quirks下启⽤与CFG Lock相关选项）           |
| Secure Boot        | 安全启动 |
| Parallel Port        | 并口 |
| Serial/COM Port        | 串⾏/COM端⼜ |

# 启⽤清单
| 名称        | 说明               |
| ----------- | ------------------- |
| VT-x  |  VT-x  |
| UEFI Boot Mode  |  UEFI启动模式。请不要使⽤Legacy  |
| 硬盘模式：改为 AHCI  |  不能⽤IDE和RST RAID  |
| Above 4G decoding  |  ⼤于4G地址空间解码  |
| Hyper-Threading  |  超线程  |
| Execute Disable Bit  |  执⾏禁⽤位  |
| EHCI/XHCI Hand-off  |  EHCI / XHCI接⼿控制  |
| OS type : Windows 8.1/10 UEFI Mode  |  操作系统类型：Windows 8.1 / 10 UEFI模式  |
| DVMT Pre-Allocated (iGPU Memory)  |  DVMT预分配（iGPU内存）： 64MB （如果能设Max就设）  |
| Legacy RTC Device  |  传统RTC设备  |

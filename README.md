# Hackintosh-OC-Lenovo-ThinkCentre-M920x

## 平台配置
* 准系统：Lenovo ThinkCentre M920x
* CPU：Intel Core i5-8600T (Coffee Lake)
* iGPU：Intel UHD Graphics 630
* dGPU：AMD Radeon RX460 4GB
* 网卡：Apple BCM94360CS2
* 内存：16GB DDR4 2666MHz

## 特性
* 仿冒机型：Macmini8,1（SN已去除，需自行补充）
* 系统版本：Big Sur 11.2.3
* 核显正常，编解码加速正常，显卡FB：3E9B0007，VRAM：1536MB
* 独显输出正常，最高支持6屏输出（MiniDPx4 + DP + HDMI）
* 内置扬声器、前置耳机、麦克风输出正常，声卡ID：17
* WiFi正常，免驱
* 蓝牙正常，支持接力，支持随航
* 睡眠正常，支持电能小憩
* USB端口正常，端口属性正确修正
* CPU电源管理正常，支持功率报告
* 支持开机音效
* 电源按钮正常，短按1S睡眠，长按>3S弹出关机对话框

## 已知问题
* EC(SuperIO)无驱动

## BIOS配置（版本：M1UKT65A）
* 恢复出厂设置（推荐使用主板CMOS跳线进行完全复位）
* 关闭VT-d
* 关闭CFG Lock：0x721 0x0
* 设置64M预分配显存：0xA44 0x2

## 更新日志
### 2021-4-30
* 去除无用的ACPI表
* 关闭Verbose模式
### 2021-4-24
* 更新OpenCore 0.6.8
* 修复HDMI接口输出

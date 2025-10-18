# OnePlus Kernels with SukiSU Ultra and SUSFS
# OnePlus 内核集成 SukiSU Ultra 和 SUSFS

[English](#english) | [中文](#中文)

---

## English

This repository provides GitHub Actions workflows to automatically build flashable AnyKernel3 ZIPs for multiple OnePlus devices with integrated SukiSU Ultra and SUSFS support.

### 🌟 Features

- **SukiSU Ultra** - Advanced kernel-level root solution
- **SUSFS (Super User File System)** - Enhanced file system security and isolation
- **Baseband Guard LSM** (Optional) - Additional security layer
- **WireGuard** - Modern VPN protocol built into the kernel
- **Magic Mount** - Advanced mounting capabilities
- **TMPFS_XATTR (Mountify)** - Extended attribute support for tmpfs
- **BBR & ECN** - Advanced TCP congestion control and network optimizations
- **sched_ext** - Extensible scheduler framework (6.6 kernels)
- **hmbird conversion** - Optimized for certain 6.6 kernel cases

### 📱 Supported Devices

#### Android 15 / Kernel 6.6

| Device | Codename |
|--------|----------|
| OnePlus 13 | `oneplus_13` |
| OnePlus 13 Global | `oneplus_13_global` |
| OnePlus 13T | `oneplus_13t` |
| OnePlus 13S | `oneplus_13s` |
| OnePlus Ace 5 Pro | `oneplus_ace5_pro` |
| OnePlus Ace 5 Ultra | `oneplus_ace5_ultra` |
| OnePlus Ace 3V | `oneplus_ace3_v` (alias of OP13T) |
| OnePlus Pad 3 | `oneplus_pad_3` |
| OnePlus Pad 2 Pro | `oneplus_pad_2_pro` |

#### Android 14 / Kernel 6.1

| Device | Codename |
|--------|----------|
| OnePlus 12 | `oneplus12_v` |
| OnePlus 13R | `oneplus_13r` |
| OnePlus Ace 5 | `oneplus_ace5` |
| OnePlus Ace 3 Pro | `oneplus_ace3_pro_v` |
| OnePlus Ace 3V | `oneplus_ace_3v_v` |
| OnePlus Nord 4 | `oneplus_nord_4_v` |
| OnePlus Nord 5 | `oneplus_nord_5` |
| OnePlus Nord CE4 Lite 5G | `oneplus_nord_ce4_lite_5g_v` |
| OnePlus Pad 2 | `oneplus_pad2_v` |
| OnePlus Pad Pro | `oneplus_pad_pro_v` |

#### Android 13 / Kernel 5.15

| Device | Codename |
|--------|----------|
| OnePlus 11 | `oneplus_11_v` |
| OnePlus Open | `oneplus_open_v` |
| OnePlus 12R | `oneplus_12r_v` |
| OnePlus Ace 2 Pro | `oneplus_ace2_pro_v` |

#### Android 12 / Kernel 5.10

| Device | Codename |
|--------|----------|
| OnePlus 11R | `oneplus_11r_v` |
| OnePlus Ace 2 | `oneplus_ace2_v` |
| OnePlus 10T | `oneplus_10t_v` |
| OnePlus 10 Pro | `oneplus_10_pro_v` |

### 🚀 Installation

1. Download the latest kernel ZIP for your device from [Releases](https://github.com/Bouteillepleine/Oneplus-Kernels-SukiSu/releases)
2. Boot into custom recovery (TWRP/OrangeFox recommended)
3. Flash the AnyKernel3 ZIP
4. Reboot and enjoy!

> ⚠️ **Warning**: Always backup your data before flashing custom kernels. Ensure you have a working recovery and know how to restore your device.

### 🔧 Build Artifacts

Each build produces:

- **Flashable AnyKernel3 ZIP** - Ready to flash kernel package
- **Build metadata** - Detailed build information and logs

### 🛠️ Building Locally

To trigger a build for a specific device, use the GitHub Actions workflow or clone and build manually:

```bash
# Clone the repository
git clone https://github.com/Bouteillepleine/Oneplus-Kernels-SukiSu.git
cd Oneplus-Kernels-SukiSu

# Follow the workflow scripts for your target device
📋 Requirements
Unlocked bootloader
Custom recovery (TWRP/OrangeFox)
Compatible OnePlus device from the supported list
Basic knowledge of flashing custom kernels
🤝 Acknowledgments
This project wouldn't be possible without:

KernelSU-Next & SukiSU Ultra & Wild+
susfs4ksu by simonpunk
AnyKernel3 by osm0sis and contributors
OnePlusOSS - Official OnePlus kernel sources
Community contributors - For testing, feedback, and improvements
📄 License
This project follows the licensing of its upstream components. Please refer to individual component licenses for details.

⚠️ Disclaimer
This is unofficial software. Use at your own risk.

The authors are not responsible for any damage to your device
Always ensure you have a backup and know how to restore your device
Warranty may be void after unlocking bootloader and flashing custom software
中文
本仓库提供 GitHub Actions 工作流，可自动为多款 OnePlus 设备构建集成 SukiSU Ultra 和 SUSFS 支持的可刷写 AnyKernel3 ZIP 包。

🌟 特性
SukiSU Ultra - 高级内核级 Root 解决方案
SUSFS (超级用户文件系统) - 增强的文件系统安全性和隔离
Baseband Guard LSM（可选）- 额外的安全层
WireGuard - 内置于内核的现代 VPN 协议
Magic Mount - 高级挂载功能
TMPFS_XATTR (Mountify) - tmpfs 的扩展属性支持
BBR & ECN - 高级 TCP 拥塞控制和网络优化
sched_ext - 可扩展调度器框架（6.6 内核）
hmbird 转换 - 针对某些 6.6 内核情况的优化
📱 支持的设备
Android 15 / 内核 6.6
设备	代号
OnePlus 13	oneplus_13
OnePlus 13 全球版	oneplus_13_global
OnePlus 13T	oneplus_13t
OnePlus 13S	oneplus_13s
OnePlus Ace 5 Pro	oneplus_ace5_pro
OnePlus Ace 5 Ultra	oneplus_ace5_ultra
OnePlus Ace 3V	oneplus_ace3_v (OP13T 的别名)
OnePlus Pad 3	oneplus_pad_3
OnePlus Pad 2 Pro	oneplus_pad_2_pro
Android 14 / 内核 6.1
设备	代号
OnePlus 12	oneplus12_v
OnePlus 13R	oneplus_13r
OnePlus Ace 5	oneplus_ace5
OnePlus Ace 3 Pro	oneplus_ace3_pro_v
OnePlus Ace 3V	oneplus_ace_3v_v
OnePlus Nord 4	oneplus_nord_4_v
OnePlus Nord 5	oneplus_nord_5
OnePlus Nord CE4 Lite 5G	oneplus_nord_ce4_lite_5g_v
OnePlus Pad 2	oneplus_pad2_v
OnePlus Pad Pro	oneplus_pad_pro_v
Android 13 / 内核 5.15
设备	代号
OnePlus 11	oneplus_11_v
OnePlus Open	oneplus_open_v
OnePlus 12R	oneplus_12r_v
OnePlus Ace 2 Pro	oneplus_ace2_pro_v
Android 12 / 内核 5.10
设备	代号
OnePlus 11R	oneplus_11r_v
OnePlus Ace 2	oneplus_ace2_v
OnePlus 10T	oneplus_10t_v
OnePlus 10 Pro	oneplus_10_pro_v
🚀 安装步骤
从 Releases 下载适合您设备的最新内核 ZIP
启动到第三方 Recovery（推荐 TWRP/OrangeFox）
刷入 AnyKernel3 ZIP 包
重启并享受！
⚠️ 警告：刷入自定义内核前请务必备份数据。确保您有可用的 Recovery 并知道如何恢复设备。

🔧 构建产物
每次构建会产生：

可刷写的 AnyKernel3 ZIP - 即刷即用的内核包
构建元数据 - 详细的构建信息和日志
🛠️ 本地构建
要为特定设备触发构建，请使用 GitHub Actions 工作流或手动克隆并构建：

Copy
# 克隆仓库
git clone https://github.com/Bouteillepleine/Oneplus-Kernels-SukiSu.git
cd Oneplus-Kernels-SukiSu

# 按照工作流脚本为您的目标设备构建
📋 要求
已解锁 Bootloader
第三方 Recovery（TWRP/OrangeFox）
支持列表中的兼容 OnePlus 设备
刷入自定义内核的基础知识
🤝 致谢
本项目离不开以下支持：

KernelSU-Next & SukiSU Ultra & Wild+
susfs4ksu by simonpunk
AnyKernel3 by osm0sis 及贡献者
OnePlusOSS - OnePlus 官方内核源码
社区贡献者 - 感谢测试、反馈和改进
📄 许可证
本项目遵循其上游组件的许可。详情请参阅各个组件的许可证。

⚠️ 免责声明
这是非官方软件，使用风险自负。

作者不对您的设备损坏负责
请务必确保您有备份并知道如何恢复设备
解锁 Bootloader 和刷入自定义软件后保修可能失效
Made with ❤️ for the OnePlus community

为 OnePlus 社区用心制作 ❤️

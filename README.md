# OnePlus Kernels with SukiSU Ultra and SUSFS

This repository provides GitHub Actions workflows to automatically build flashable AnyKernel3 ZIPs for multiple OnePlus devices with integrated SukiSU Ultra and SUSFS support.

## 🌟 Features

- **SukiSU Ultra** - Advanced kernel-level root solution
- **SUSFS (Super User File System)** - Enhanced file system security and isolation
- **Baseband Guard LSM** (Optional) - Additional security layer
- **WireGuard** - Modern VPN protocol built into the kernel
- **Magic Mount** - Advanced mounting capabilities
- **TMPFS_XATTR (Mountify)** - Extended attribute support for tmpfs
- **BBR & ECN** - Advanced TCP congestion control and network optimizations
- **sched_ext** - Extensible scheduler framework (6.6 kernels)
- **hmbird conversion** - Optimized for certain 6.6 kernel cases

## 📱 Supported Devices

### Android 15 / Kernel 6.6

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

### Android 14 / Kernel 6.1

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

### Android 13 / Kernel 5.15

| Device | Codename |
|--------|----------|
| OnePlus 11 | `oneplus_11_v` |
| OnePlus Open | `oneplus_open_v` |
| OnePlus 12R | `oneplus_12r_v` |
| OnePlus Ace 2 Pro | `oneplus_ace2_pro_v` |

### Android 12 / Kernel 5.10

| Device | Codename |
|--------|----------|
| OnePlus 11R | `oneplus_11r_v` |
| OnePlus Ace 2 | `oneplus_ace2_v` |
| OnePlus 10T | `oneplus_10t_v` |
| OnePlus 10 Pro | `oneplus_10_pro_v` |

## 🚀 Installation

1. Download the latest kernel ZIP for your device from [Releases](https://github.com/Bouteillepleine/Oneplus-Kernels-SukiSu/releases)
2. Boot into custom recovery (TWRP/OrangeFox recommended)
3. Flash the AnyKernel3 ZIP
4. Reboot and enjoy!

> ⚠️ **Warning**: Always backup your data before flashing custom kernels. Ensure you have a working recovery and know how to restore your device.

## 🔧 Build Artifacts

Each build produces:

- **Flashable AnyKernel3 ZIP** - Ready to flash kernel package
- **Build metadata** - Detailed build information and logs

## 🛠️ Building Locally

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
Made with ❤️ for the OnePlus community

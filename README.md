OnePlus Kernels with SukiSU Ultra and SUSFS. 
This repo provides GitHub Actions workflows to build flashable AnyKernel3 ZIPs for multiple OnePlus devices and optionally publish prereleases.

Overview

Build targets: Multiple OnePlus models 

SukiSU Ultra
SUSFS 
Optional Baseband Guard LSM
WireGuard, Magic Mount, TMPFS_XATTR (Mountify), BBR, ECN options
sched_ext for 6.6 kernels, hmbird conversion for certain 6.6 cases
Output: Flashable AnyKernel3 ZIP and build metadata artifacts

Android 15 / 6.6: oneplus_13, oneplus_13_global, oneplus_13t, oneplus_13s, oneplus_ace5_pro, oneplus_pad_3, oneplus_pad_2_pro, oneplus_ace3_v (alias of OP13T), oneplus_ace5_ultra
Android 14 / 6.1: oneplus12_v, oneplus_13r, oneplus_ace5, oneplus_pad2_v, oneplus_ace3_pro_v, oneplus_nord_4_v, oneplus_ace_3v_v, oneplus_nord_5, oneplus_pad_pro_v, oneplus_nord_ce4_lite_5g_v
Android 13 / 5.15: oneplus_11_v, oneplus_open_v, oneplus_12r_v, oneplus_ace2_pro_v
Android 12 / 5.10: oneplus_11r_v, oneplus_ace2_v, oneplus_10t_v, oneplus_10_pro_v

Acknowledgments
KernelSU-Next, SukiSU Ultra
susfs4ksu by simonpunk
AnyKernel3 by osm0sis and contributors
OnePlusOSS kernel manifests
Community contributors

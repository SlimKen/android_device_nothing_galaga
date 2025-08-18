### Custom Recovery Tree for the Nothing CMF Phone 2 pro (Galaga)

```
# SPDX-License-Identifier: Apache-2.0
```

#### The Linux Kernel binary and it's accompanying modules are provided by [Nothing Technology Limited](https://github.com/NothingOSS) under the GNU Public License


=========================================

The Nothing CMF Phone 2 pro (codenamed _"Galaga"_) is a mid-range smartphone from Nothing released in mid 2025.

![Nothing CMF Phone 2 pro](https://fdn2.gsmarena.com/vv/pics/nothing/nothing-cmf-phone-2-pro-1.jpg)

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | 4 x 2.5 GHz Cortex-A78 & 4 x 2.0 GHz Cortex-A55
Chipset | Mediatek Dimensity 7300 pro
GPU     | Mali-G615 MC2
Memory  | 8 GB RAM
Shipped Android Version | 15 with NothingOS 3.2
Storage | 128/256 GB
Battery | Li-Po 5000 mAh, non-removable
Display | 1080 x 2392 pixels, 6.77 inches, 60/120 hz HDR10+

## Checks

Blocking checks

    [ ] Correct screen/recovery size
    [ ] Working Touch, screen
    [ ] Backup to internal/microSD
    [ ] Restore from internal/microSD
    [ ] reboot to system
    [ ] ADB

Medium checks

    [ ] update.zip sideload
    [ ] UI colors (red/blue inversions)
    [ ] Screen goes off and on
    [ ] F2FS/EXT4 Support, exFAT/NTFS where supported
    [ ] all important partitions listed in mount/backup lists
    [ ] backup/restore to/from external (USB-OTG) storage
    [ ] decrypt /data
    [ ] Correct date
    [ ] USB-OTG (flash drive)

Minor checks

    [ ] MTP export
    [ ] reboot to bootloader
    [ ] reboot to recovery
    [ ] poweroff
    [ ] battery level
    [ ] temperature
    [ ] encrypted backups
    [ ] input devices via USB (USB-OTG) - keyboard and mouse
    [ ] USB mass storage export
    [ ] set brightness
    [ ] vibrate
    [ ] screenshot
    [ ] partition SD card (No SD card slot)
    [ ] Fastbootd


## After you've built a custom recovery using this tree, you can enter the following command in fastboot to flash it

```
fastboot flash vendor_boot vendor_boot.img
```

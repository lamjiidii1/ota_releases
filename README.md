## LineageOS 20.0 for Xiaomi 12X Installation instructions

**GENERAL INFORMATION:**
- ROM: `LineageOS`
- Device: `2112123AG`
- Device codename: `psyche`
- Version: `20.0`
- Variant: `VANILLA`

**First time installation:**
- Make sure you backup your data
- Download needed stuff (rom_archive.zip, boot.img, dtbo.img and vendor_boot.img)
- Install LineageOS recovery via fastboot : 
  - `fastboot flash boot_ab boot.img`
  - `fastboot flash dtbo_ab dtbo.img`
  - `fastboot flash vendor_boot_ab vendor_boot.img`

- Then reboot into recovery via fastboot: ("`  fastboot reboot recovery  `") or by power and Vol+
- When get booted to recovery tap Factory Reset, then Format data / factory reset and continue with the formatting process. This will remove encryption and delete all files stored in the internal storage
- Return to the main menu and reboot into recovery
- Sideload the LineageOS .zip:
On the device, select “Apply Update”, then “Apply from ADB” to begin sideload
On the host machine, sideload the package using: `adb sideload filename.zip`.
- Reboot

**Update to newer release:**
- Make sure you backup your data
- Boot into recovery 
- Sideload the LineageOS .zip:
On the device, select “Apply Update”, then “Apply from ADB” to begin sideload
On the host machine, sideload the package using: `adb sideload filename.zip`
- Reboot

**NOTES:**
- Make sure to flash newer recovery with each release to stay updated
- Custom RECOVERy's are not supported in any way
- Encryption Enabled by default
- Don't seek support if you modify the ROM in any way including magisk and gapps.
- Please report bugs with logs if you found any.

**Special Thanks:**
- [SebaUbuntu](https://github.com/SebaUbuntu) For Common Trees
- [mickaelmendes50](https://github.com/mickaelmendes50/) & [Moonlight4004](https://github.com/Moonlight4004) For Fixing UDFPS and for their help
- All the guys who worked on xiaomi-sm8250 platforme

**Sources:**
- [Device tree](https://github.com/lamjiidii1/android_device_xiaomi_psyche)  | `lineage-20` branch
- [Kernel tree](https://github.com/lamjiidii1/android_kernel_xiaomi_sm8250)  | `lineage-20` branch
- [Hardware tree](https://github.com/lamjiidii1/android_hardware_xiaomi)  | `lineage-20` branch
- [Vendor tree](https://gitlab.com/lamjiidii1/android_vendor_xiaomi_psyche)  | `lineage-20` branch

**Ask for help:**
- Our Group on [Telegram](https://t.me/psychediscussion)
- My Personal [Telegram](https://t.me/lamjiidii1) Account

**Download:**
- [Github Releases](https://github.com/lamjiidii1/ota_releases/releases)

**Donate:**
- If you found this helpful, please consider supporting development with a [PayPal donation](https://www.paypal.com/paypalme/lamjiidii1). All support is appreciated.

# OrangeFox Recovery for Samsung Galaxy Tab A7 Wi-Fi (gta4lwifi)

## Introduction
This is an unofficial build of OrangeFox Recovery for the Samsung Galaxy Tab A7 Wi-Fi (SM-T500 / `gta4lwifi`). It provides advanced recovery features, custom partition flashing, and seamless OTA management.

## Features
- Full OrangeFox Recovery functionality
- Up-to-date decryption and file manager features
- Added options to directly flash `.img` files from the recovery UI to the following partitions:
  - `dtbo`
  - `vbmeta`
  - `vbmeta_system`
  - `vendor_boot`
  - `system_ext`
  - Out-of-the-box **Black theme with Google Blue accent**.
- Correctly preserved Samsung `SEANDROIDENFORCE` boot signatures to prevent bootloader panics.
- Included `flash.tar` combo file to easily flash both Recovery and VBMeta disabler simultaneously via Odin/Heimdall, avoiding AVB verification issues.

## Installation

### Prerequisites
- Samsung Galaxy Tab A7 Wi-Fi (`gta4lwifi`)
- Unlocked Bootloader (Ensure `OEM LOCK: OFF` and `KG STATUS: NORMAL` or `COMPLETED` in Download Mode)
- PC with Odin (Windows) or `odin4`/Heimdall (Linux/macOS)

### First-time Installation (via Odin / Download Mode)
1. Boot your tablet into **Download Mode** (Power off, hold Volume Up + Volume Down, and plug in the USB cable).
2. Open Odin (or `odin4` / Heimdall) on your PC.
3. Load the `flash.tar` file into the **AP** slot. *(This file contains both the OrangeFox recovery and the vbmeta disabler required to bypass AVB).*
4. Start the flash.
5. As soon as the screen goes black, hold **Power + Volume Up** to force the tablet to boot directly into Recovery Mode. Do not let it boot into Android until you've successfully entered OrangeFox.

### Updating from an Existing Custom Recovery
If you already have TWRP or an older version of OrangeFox installed:
1. Boot into Recovery Mode.
2. Select the `OrangeFox-R12.0_3-Unofficial-gta4lwifi.zip` file and swipe to install.
3. The device will automatically reboot into the newly updated OrangeFox recovery.

## Usage
- **Flashing Partition Images:** To flash GSI ROMs or custom partition images, simply tap on any `.img` file in the OrangeFox file manager. You will be prompted with a list of partitions to flash it to (now including `dtbo`, `vbmeta`, `vendor_boot`, and `system_ext`).
- **Rooting:** Magisk can be installed directly from the OrangeFox menu or by flashing a Magisk `.zip` file.

---
**Disclaimer:** Flash at your own risk. This project is provided as-is without any warranties. Make sure to back up your data before proceeding.

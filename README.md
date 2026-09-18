# OrangeFox Recovery for Samsung Galaxy Tab A7 Wi-Fi (gta4lwifi)

## Introduction
This is an unofficial build of OrangeFox Recovery for the Samsung Galaxy Tab A7 Wi-Fi (SM-T500 / `gta4lwifi`). It provides advanced recovery features, custom partition flashing, and seamless OTA management.

## Installation

### Prerequisites
- Samsung Galaxy Tab A7 Wi-Fi (`gta4lwifi`)
- Unlocked Bootloader (Ensure `OEM LOCK: OFF` and `KG STATUS: NORMAL` or `COMPLETED` in Download Mode)
- Flashing Tool, choose one of the following:
  - **Brokkr App** for Android/Linux ([GitHub Repository](https://github.com/Gabriel2392/brokkr-flash))
  - **Odin3** for Windows ([Download](https://odindownload.com/))
  - **odin4** for Linux ([Download from XDA](https://xdaforums.com/t/official-samsung-odin-v4-1-2-1-dc05e3ea-for-linux.4453423/))
  - **Heimdall** for Linux/macOS ([GitHub Repository](https://github.com/Benjamin-Dobell/Heimdall))

### Installation (via Download Mode)
1. Boot your tablet into **Download Mode** (Power off. hold Volume Up + Volume Down and plug in with the tablet using the USB cable ( other end must be connected with PC or Phone).
2. Open your preferred flashing tool (Brokkr, Odin, odin4, or Heimdall).
3. Load the `Recovery and VBMeta.tar` file into the **AP** slot. *(This file contains both the OrangeFox recovery and the vbmeta disabler required to bypass AVB).*
4. Start the flash.
5. Done, you can boot into recovery (OrangeFox).

### Updating from an Existing Custom Recovery
If you already have TWRP or an older version of OrangeFox installed:
1. Boot into Recovery Mode.
2. Select the `OrangeFox-R12.0_3-Unofficial-gta4lwifi.zip` file and swipe to install.
3. The device will automatically reboot into the newly updated OrangeFox recovery.

---
**Disclaimer:** Flash at your own risk. This project is provided as-is without any warranties. Make sure to back up your data before proceeding.

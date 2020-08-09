# HP ProBook 430/440/450 G6 Hackintosh

## Configuration
| Specifications      | Detail                       |
|---------------------|------------------------------|
| CPU                 | Intel(R) Core(TM) i5-8265U   |
| Integrated Graphics | Intel UHD Graphics 620       |
| Sound Card          | Realtek ALC236 (layout-id:3) |
| Wireless Card       | Intel Wireless               |

## MacOS Versions Supported:
- macOS 10.13 High Sierra (not tested)
- macOS 10.14 Mojave (not tested)
- macOS 10.15 Catalina
- macOS 11.00 Big Sur (Beta)

## What is Working?
- Native CPU Power Management
- Sleep/Wake
- Intel Graphics
- Audio (AppleALC)
- Trackpad (gestures)
- Type-C + Video and Audio
- HDMI Video and Audio
- USB 3.0
- Battery Management (thanks to [anor4k](https://www.tonymacx86.com/threads/guide-how-to-patch-dsdt-for-working-battery-status.116102/page-500#post-2021126) and [e285ne](https://www.tonymacx86.com/threads/guide-hp-probook-430-g6-whiskey-lake.282302/page-6#post-2147595))
- Brightness
- Brightness fn keys (if not working, turn off the laptop and hold the power button for 30 seconds to reset EC)
- Built-in camera
- Built-in mic
- Bluetooth Intel
- Intel wireless ([itlwm](https://github.com/OpenIntelWireless/itlwm) + [HeliPort](https://github.com/OpenIntelWireless/HeliPort)/[
Black80211](https://github.com/usr-sse2/Black80211-Catalina)(Catalina only))
- Fn keys: play/pause, prt scr(F13), sound mute/-/+, sleep

## Not working:
- Fingerprint reader
- SD Card Reader

## For 440/450 users:
- Disable **USBPorts.kext** and remap USB with **USBInjectAll.kext**

## Known issues:
- BIOS RTC error after sleep and reboot

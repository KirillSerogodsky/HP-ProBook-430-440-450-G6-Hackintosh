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
- macOS 11.00 Big Sur

## What is Working?
- [x] Native CPU Power Management
- [x] Sleep/Wake
- [x] Intel Graphics
- [x] Audio
- [x] Trackpad (gestures)
- [x] Type-C + Video and Audio
- [x] HDMI Video and Audio
- [x] USB 3.0
- [x] Battery Management (thanks to [anor4k](https://www.tonymacx86.com/threads/guide-how-to-patch-dsdt-for-working-battery-status.116102/page-500#post-2021126) and [e285ne](https://www.tonymacx86.com/threads/guide-hp-probook-430-g6-whiskey-lake.282302/page-6#post-2147595))
- [x] Brightness
- [x] Brightness fn keys (if not working, turn off the laptop and hold the power button for 30 seconds to reset EC)
- [x] Built-in camera
- [x] Built-in mic
- [x] Bluetooth Intel
- [x] Intel wireless ([itlwm](https://github.com/OpenIntelWireless/itlwm) + [HeliPort](https://github.com/OpenIntelWireless/HeliPort)/[
Black80211](https://github.com/usr-sse2/Black80211-Catalina))
- [x] Fn keys: play/pause, prt scr(F13), sound mute/-/+, sleep

## Not working:
- [ ] Fingerprint reader
- [ ] SD Card Reader
- [ ] Line-in mic (checking and fixing daemon script)

## For 440/450 users:
- Disable **USBPorts.kext** and remap USB with **USBInjectAll.kext**
- Possibly need change layout-id in boot-args

## IMPORTANT
Make sure to add SMBIOS of MacBook Pro 15.2 and serial number in config.plis.

## Known issues:
- BIOS RTC error after sleep and reboot

# HP ProBook 430/440/450 G6 Hackintosh

## Configuration

| Specifications      | Detail                       |
| ------------------- | ---------------------------- |
| CPU                 | Intel(R) Core(TM) i5-8265U   |
| Integrated Graphics | Intel UHD Graphics 620       |
| Sound Card          | Realtek ALC236 (layout-id:3) |
| Wireless Card       | Intel Wireless               |

## MacOS Versions Supported:
- macOS 10.15 Catalina
- macOS 11.00 Big Sur

## What is Working?
- [x] Native CPU Power Management
- [x] Sleep/Wake
- [x] Intel Graphics
- [x] Audio
- [x] Trackpad (gestures)
- [x] Type-C USB
- [x] Type-C: video and audio
- [x] HDMI: video and audio
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

## Wifi Setup:
- [ ] download [HeliPort](https://github.com/OpenIntelWireless/HeliPort/releases/download/v1.0.0/HeliPort.dmg) and install the app  , run app and fun . 
- [ ] you can make the  HeliPort app run every startaup by Following this Guide [Open items automatically when you log in on Mac](https://support.apple.com/guide/mac-help/open-items-automatically-when-you-log-in-mh15189/mac)

## Not working:
- [ ] Fingerprint reader
- [ ] SD Card Reader
- [ ] Line-in mic (checking and fixing daemon script)

## BIOS settings
- [ ] Fast Boot
- Secure Boot Configurations - Configure Legacy Support and Secure Boot = Legacy Support Disable and Secure Boot Disable
- [ ] VTx in System Options
- Wake On LAN = Disabled
- Wake On WLAN = Disabled
- Video Memory size = 64 MB
- [ ] Fingerprint Device
- [ ] Media Card Reader in Port Options
- Wake on USB = optional

## For 440/450 users:
- Disable **USBPorts.kext** and remap USB with **USBInjectAll.kext** using **[Dortania guide](https://dortania.github.io/OpenCore-Post-Install/usb/intel-mapping/intel.html)** or **[Hackintool](https://www.tonymacx86.com/threads/release-hackintool-v3-x-x.254559/)**.
- Possibly need change layout-id in boot-args for **AppleALC.kext**

## IMPORTANT
Make sure to add SMBIOS of MacBook Pro 15.2 and serial number in config.plis.

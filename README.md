# HP ProBook 430 G6 Hackintosh

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
- Battery Management
- Brightness keys (if not working, turn off the laptop and hold the power button for 30 seconds to reset EC)
- Built-in camera
- Built-in mic
- Bluetooth Intel
- Intel wireless ([itlwm](https://github.com/OpenIntelWireless/itlwm) + [HeliPort](https://github.com/OpenIntelWireless/HeliPort)/[
Black80211](https://github.com/usr-sse2/Black80211-Catalina)(Catalina only))

## Not working:
- Fingerprint reader
- SD Card Reader

## Known issues
- BIOS RTC error after sleep and reboot

# Lenovo-B50-80-Hackintosh-OpenCore

## What's Working...
 - [x] Audio & headphone jack
 - [x] CPU Speedstep (XCPM)
 - [x] Fully Functional iGPU QE/CI Enabled Graphics
 - [x] Battery Management
 - [x] Ethernet
 - [x] HDMI + Audio
 - [x] Smart Touchpad + Gestures (using I2C)
 - [x] WebCam + Integrated Mic
 - [x] Usb 3.0 + Usb 2.0
 - [x] WiFi + Bluetooth
 - [x] Native hotkey support with Fn keys

### Laptop configuration


- **Audio** : The Sound Card is `Realtek ALC233`, which is driven by `AppleALC` on `layout-id 28`. It supported using `AppleALC.kext` + custom generated using SSDTTime `SSDT-HPET.aml` + `SSDT-EC.aml`

- **CPU** : The CPU model is `i5-5020U` and XCPM power management is natively supported.

- **Graphics** : The iGPU is `Intel HD Graphics 5500`, and its enabled using `Ig-Platform-id=06002616`, `device-id=16160000`, `framebuffer-fbmem=00009000`, `framebuffer-patch-enable=01000000` and `framebuffer-stolenmem=00003001`.

- **Battery** : Battery Management using `SMCBatteryManager.kext`.

- **Touchpad** : Elan Touchpad. Supported using `VoodooI2C.kext` + `VoodooI2CHID.kext`

- **Keyboard** : PS2. Supported using `VoodooPS2Controller.kext`

- **USBs** :  Supported using `VoodooPS2Controller.kext`

- **Ethernet** : Gigabit Ethernet using `RealtekRTL8111.kext`.

- **HDMI** : Working using `WhateverGreen.kext`.

- **Wi-Fi** : Stock WiFi Card is `Intel Wireless AC 3160`. It supported using `AirportItlwm.kext`

- **Bluetooth** : Stock `Intel Wireless AC 3160`. Supported using `IntelBluetoothFirmware.kext` + `IntelBluetoothInjector.kext`

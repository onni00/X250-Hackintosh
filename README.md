# X250-Hackintosh

macOS for ThinkPad X250 (Mojave & Catalina)

## Pre-Installation

### 1. BIOS settings

### BIOS settings

| Item | Setting |
| ------------- | ------------ |
| Config/Network/Wake On Lan | Disabled |
| USB UEFI BIOS Support | Enabled |
| Always On USB | Disabled |
| USB 3.0 Mode | Enabled |
| Power Intel Rapid Start Technology | Disabled |
| Serial SATA Controller Mode Option | AHCI |
| Security Predesktop Authentication | Disabled |
| Security Chip | Disabled |
| Memory Protection Execution Prevention | Enabled |
| Virtualization | Disabled |
| Fingerprint Reader | Disabled |
| Anti Theft | Disabled |
| Computrace | Disabled |
| Secure Boot | Disabled |
| Startup Network Boot | PCI Lan |
| UEFI/Legacy Boot | UEFI Only |
| CSM Support | Disabled |
| Boot Mode | Quick |

### 3. Hardware

|Compenent|Reference|
|---|---|
|CPU|Intel Core i5-5200U|
|RAM|DDR3L 8GB Bus 1600MHz|
|GFX|Intel HD Graphics 5500|
|Sound|Realtek ALC292|
|Display|12.5" FHD IPS LCD|
|WIFI|Dell DW1820A|

#### What will work

- Power Management (C/P-States, Fan RPM, Speedstep, etc)
- HD Intel Graphic Card (HD5500)
- Sleep (Sleep from menu + lid close sleep)
- Camera
- Ethernet
- Battery Status
- Brightness
- Keyboard, Trackpad and Trackpoint
- Sound (automatic headphone detection, mute, volume controls fully working)
- USB Ports
- SD Card Reader
- Bluetooth

#### Not working

- Fingerprint Reader
- VGA

#### WIFI

Inbuilt Intel WiFi won't work out of the box.

- Broadcom BCM94360CSAX & NGFF A/E Adapter - 802.11a/b/g/n 2.4 GHz & 5 GHz (Recommended Upgrade)
- Dell DW1820A – 802.11a/b/g/n 2.4 GHz & 5 GHz (Broadcom)
- Dell DW1560 - 802.11a/b/g/n 2.4 GHz & 5 GHz (Broadcom)
- Dell DW1830 – 802.11ac 2.4 GHz & 5 GHz (Broadcom)

## Installation

....

## Post-Installation

### 1. Tools needed

- Clover

### 2. Kexts used

- AirportBrcmFixup.kext (for DW1820A and DW1560)
- ACPIBatteryManager.kext
- AppleALC.kext --> i fix with VoodooHDA.kext
- BrcmBluetoothInjector.kext (requires for BrcmPatchRAM3.kext)
- BrcmFirmwareData.kext
- BrcmPatchRAM2.kext (BrcmPatchRAM3.kext for Catalina)
- EFICheckDisabler.kext
- FakeSMC.kext
- IntelMausi.kext
- Lilu.kext
- USBPorts.kext
- VoodooPS2Controller.kext
- VoodooInput.kext
- WhateverGreen.kext

### 3. Patched
patch to /ACPI/patched/


credits

- Paypal: <https://www.paypal.me/thebinhluong0519>
- Ethereum: 0xC202255193D95979A7C937aA3CB5220FAD9E2aBe

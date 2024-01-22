# TWRP Device tree for Poco M5

[![SourceForge Total Downloads](https://img.shields.io/sourceforge/dt/orangefox-device-xiaomi-rock?style=social&logo=sourceforge&logoColor=%23000000)](https://sourceforge.net/projects/premiumprjktrom/files/Rock/OrangeFox-UNOFFICIAL-rock_01032024.img/download)

Poco M5 (codenamed _"rock/stone"_) is a smartphone from Xiaomi.

It was announced & released on September 2022.

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
SoC     | Mediatek Helio G99 (MT6789) (6nm)
CPU     | Octa-core (2x2.2 GHz Cortex-A76 & 6x2.0 GHz Cortex-A55)
GPU     | Mali-G57 MC2
Memory  | 4 GB RAM
Shipped Android Version | 12.0 with MIUI 13
Storage | 64/128 GB
Battery | Li-Po 5000 mAh, non-removable
Display | IPS LCD, 90Hz, 500 nits (HBM), 6.58 inches, 104.3 cm2 (~83.6% screen-to-body ratio), 1080 x 2408 pixels, 20:9 ratio (~401 ppi density), Corning Gorilla Glass 3.
Camera  | 50 MP, f/1.8, (wide), PDAF, 2 MP, f/2.4, (macro), 2 MP, f/2.4, (depth)

## Device picture

![1704331359766](https://github.com/TeamWin/android_device_xiaomi_fleur/assets/142644567/e20900e9-0a2e-43f3-bc5c-244984ea0b73)

## Features

Works:

- [X] ADB
- [X] Decryption
- [X] Display
- [X] Fasbootd
- [X] Flashing
- [X] MTP
- [X] Sideload
- [X] USB OTG
- [X] SD Card
- [X] Touch
- [ ] Flashlight
- [ ] Vibrator

# Building
```bash
source build/envsetup.sh
lunch twrp_rock-eng
mka vendorbootimage
```

## To use it:

```
fastboot flash vendor_boot out/target/product/rock/vendor_boot.img
```

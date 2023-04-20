
  

## EFI-OPENCORE-I5-6600K-GTX-1070-PASCAL

  

OPENCORE 0.8.5 EFI using I5 6600K and Nvidia GTX 1070

  

![nfo](https://cdn.discordapp.com/attachments/778932989693526038/1098634738614403232/EFI_1070.png)

  

**Latest tested macOS**: Ventura 13.2

  

**Current OpenCore**: 0.8.5

  
See [documentation](https://dortania.github.io/GPU-Buyers-Guide/modern-gpus/nvidia-gpu.html#pascal-series-gtx-10xx)

  
  

## Complete hardware specs

  

- Intel i5 6600K
- MSI B250M PRO-VDH
- EVGA GTX 1070
- 16GB RAM Corsair Dominator Platinum - 3200 MHz DDR4

  

## What works

  

- macOS Monterey 13.2

- WiFi (using [itlwm](https://github.com/OpenIntelWireless/itlwm) + [heliport](https://github.com/OpenIntelWireless/HeliPort))

- Audio
- HDMI/DP
- All USB ports
- 2x 2.5Gbit Ethernet
- Everything iCloud related (Drive, iMessage, Facetime, etc)
- DRM content (Netflix, ATV+, Airplay 2 mirroring etc)
- Shutdown/Reboot
- Deep Sleep

  

## What doesn't work

  

- (oob) WiFi and Bluetooth + Airdrop + Sidecar..
*(will be fixed with BCM94360CD card)*

  

## Kexts used:

  

- Lilu.kext
- itlwm.kext
- Lilu.kext
- USBInjectAll.kext
- VirtualSMC.kext
- WhateverGreen.kext
-  *Other Kext needed for my config (and residuals)*

## Boot-args

ngfxcompat=1 **Ignore compatibility check in NVDAStartupWeb**
ngfxgl=1 **Disable Metal support on NVIDIA**

## How to use it ?

  

⚠️ Dont forget to recreate the _plateforminfo_ section and change SMBIOS data (using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) or any other tool) ⚠️

  
## Thanks/Credits

  
- [Opencore Team](https://dortania.github.io/getting-started/)

### Disclaimer 
*Some residual SSTD or Kext may be present but not used (the same EFI is used on different hardware configurations)*
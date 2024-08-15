# *EFI OC Z590 AORUS PRO AX macOS Ventura / Sonoma*


[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Gilberto-Mascena/Z590-AORUS-PRO-AX)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Gilberto-Mascena/Z590-AORUS-PRO-AX/.github%2Fworkflows%2Fbuild.yml)
[![license](https://img.shields.io/github/license/Gilberto-Mascena/Z590-AORUS-PRO-AX)](https://github.com/Gilberto-Mascena/Z590-AORUS-PRO-AX/blob/main/LICENSE.md)
[![GitHub stars](https://img.shields.io/github/stars/Gilberto-Mascena/Z590-AORUS-PRO-AX)](https://github.com/Gilberto-Mascena/Z590-AORUS-PRO-AX/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/Gilberto-Mascena/Z590-AORUS-PRO-AX)](https://github.com/Gilberto-Mascena/Z590-AORUS-PRO-AX/issues)
[![tag](https://img.shields.io/github/v/release/Gilberto-Mascena/Z590-AORUS-PRO-AX?include_prereleases)](https://github.com/Gilberto-Mascena/Z590-AORUS-PRO-AX/releases)
![release](https://img.shields.io/github/release-date/Gilberto-Mascena/Z590-AORUS-PRO-AX)
![size](https://img.shields.io/github/repo-size/Gilberto-Mascena/Z590-AORUS-PRO-AX)

---

## *Operational system*

<img align="right" src="./img/bannerp.png" alt="photo Z590 AORUS PRO AX" width="330">

_**macOS**  **Sonoma 14.6.1**_

---

_**My Setup**_

---

- _**Motherboard**_
  - <a href="https://www.gigabyte.com/br/Motherboard/Z590-AORUS-PRO-AX-rev-10#kf" target="_blank">*Gigabyte Z590 AORUS PRO AX*</a>
- _**Bios version**_
  - *F11*
- _**Case**_
  - *Fortress-tg Gamemax*
- **Power supply**
  - *SUPER FLOWER - LEGION GX PRO 750W 80 PLUS GOLD*
- _**CPU**_
  - *Core i9 11900K (QV1K es)*
- _**Water Cooler**_
  - *SUPER FRAME SF-W360*
- _**NVME M.2**_
  - *XPG GAMMIX S41 512GB / macOS*
- _**NVME M.2**_
  - *XPG GAMMIX S41 512GB / Windows 11*
- _**NVME M.2**_
  - *XPG GAMMIX S11L 256GB / Ubuntu*
- _**GPU**_
  - *XFX AMD Radeon RX 6600 SWFT 210*
- _**Memory**_
  - *CORSAIR VENGEANCE LPX 4x16GB 64GB*
- _**WI-FI / Bluetooth**_
  - *Intel AX200*
- _**Network**_
  - *Intel I225-V*  
---

<a name="ancora"></a>
## Topic navigation
- [*What works*](#ancora1)
- [*Geekbench results*](#ancora2)
- [*Screenshot*](#ancora3)
- [*Kexts used, (all Releases)*](#ancora4)
- [*Recommended tools*](#ancora5)
- [*Intel BIOS Settings*](#ancora6)
- [*Thanks*](#ancora7)
- [*License* ](#ancora8)

---

<a id="ancora1"></a>
## *What works*

- [x] *Sound*
- [x] *Network*
- [x] *WI-FI*
- [x] *Bluetooth*
- [x] *USB*
- [x] *Sleep*

[Top](#ancora)

---

<a id="ancora2"></a>
## *Geekbench results*

* _**CPU QV1K es**_
  *As it is an engineering processor, it requires an activation key [`Geekbench`](https://www.geekbench.com) to generate the tests, I don't have it!*

[Top](#ancora)

---

<a id="ancora3"></a>
## *Screenshot*

![about-mac-Ventura](./img/about-Ventura.png)
---
![about-mac-Sonoma](./img/about-Sonoma.png)
## *Sound*
![sound](./img/sound.png)
## *Wired Network and WI-FI*
![network](./img/network-wifi.png)
## *Bluetooth*
![bluetooth](./img/bluetooth.png)
## *Hackintool Peripherals*
![peripherals](./img/peripherals.png)
## *Hackintool OpenCore Version*
![opencore-version](./img/opencore-version.png)
## *Hackintool kexts*
![kexts](./img/kexts.png)
## *Hackintool USB port mapping*
![usb-mapping](./img/USB-mapping.png)

[Top](#ancora)

---

<a id="ancora4"></a>
## *Kexts used, (all Releases)*

- *[`WhateverGreen.kext`](https://github.com/acidanthera/WhateverGreen)*
- *[`Lilu.kext`](https://github.com/acidanthera/Lilu)*
- *[`VirtualSMC`](https://github.com/acidanthera/VirtualSMC), only: `VirtualSMC.kext`, `SMCProcessor.kext` and `SMCSuperIO.kext`*.
- *[`AppleInteli210Ethernet.kext`](https://github.com/luchina-gabriel/youtube-files/raw/main/AppleIntelI210Ethernet.kext.zip)*
- *[`AppleIGC.kext`](https://github.com/SongXiaoXi/AppleIGC) as an option if your internet connects but you can't browse, remove AppleInteli210Ethernet.kext and do an OC Clean Snapshot, this should    solve your internet problem* 
- *[`CpuTscSync.kext`](https://github.com/acidanthera/CpuTscSync)*
- *`USBMap.kext`*
- *[`AirportItlwm.kext`](https://github.com/OpenIntelWireless/itlwm/releases) use the version corresponding to macOS*
- *[`BluetoolFixup.kext`](https://github.com/acidanthera/BrcmPatchRAM/releases)*
- *[`IntelBluetoothFirmware.kext`](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)*
- *[`IntelBTPatcher.kext`](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)*

[Top](#ancora)

---

<a id="ancora5"></a>
## *Recommended tools*

* _**Recommendation 1**_
  * *Use [`GenSMBIOS`](https://github.com/corpnewt/GenSMBIOS), to generate new serials for your SMBIOS in order to avoid conflicts with iServices.*
* _**Recommendation 2**_
  * *Use [`ProperTree`](https://github.com/corpnewt/ProperTree), to edit your config.plist.*     
* _**Recommendation 3**_
  * *Use [`USBMap`](https://github.com/corpnewt/USBMap), to map your USB ports, starting from OC 0.9.3, they can be mapped with XHCIPortLimit enabled in config.plist + [`USBInjectAll`](https://github.com/Sniki/OS-X-USB-Inject-All/releases).*
* _**Recommendation 4**_
  * *Extract your DSDT from windows.*
  * *Use [`SSDTTime`](https://github.com/corpnewt/SSDTTime), generate your SSDT patches.*    
* _**Recommendation 5**_
  * *Use [`MaciASL`](https://github.com/acidanthera/MaciASL), to compile your patches on mac SSDT.*
* _**Recommendation 6**_
  * *Use [`MountEFI`](https://github.com/corpnewt/MountEFI/blob/update/Mount%20EFI%20Automator%20Quick%20Action.zip), to mount EFI on macOS.*

[Top](#ancora)

---

<a id="ancora6"></a>
## *Intel BIOS Settings*

- [*OpenCore Install Guide*](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#intel-bios-settings)

[Top](#ancora)

---

<a id="ancora7"></a>
## *Thanks*

- [*Acidanthera Team*](https://github.com/acidanthera)
- [*CorpNewt*](https://github.com/corpnewt)
- [*CrisHotpatch*](https://t.me/crishotpatch)
- [*Dortania*](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo)
- [*Dicas do Mateus*](https://www.youtube.com/c/DicasdoMateus)
- [*Gabriel Luchina*](https://www.youtube.com/c/gabrielluchina)
- [*AppleIGB*](https://github.com/Shaneee/AppleIGB)
- [*AppleIGC*](https://github.com/SongXiaoXi/AppleIGC?tab=readme-ov-file)
- *And others*

[Top](#ancora)

---

<a id="ancora8"></a>
## *License* 

*The* [*MIT License*](./LICENSE.md) (*MIT*)

*Copyright :copyright: 2023* 

[Top](#ancora)

---
# *EFI OC Z590 AORUS PRO AX macOS Ventura*



![tag](https://img.shields.io/github/v/release/Gilberto-Mascena/Z590-AORUS-PRO-AX?include_prereleases)
![release](https://img.shields.io/github/release-date/Gilberto-Mascena/Z590-AORUS-PRO-AX)
![size](https://img.shields.io/github/repo-size/Gilberto-Mascena/Z590-AORUS-PRO-AX)
![license](https://img.shields.io/github/license/Gilberto-Mascena/Z590-AORUS-PRO-AX)
##

## *Sistema Operacional*

<img align="right" src="./img/banner.png" alt="Z590 AORUS PRO AX" width="330">

*macOS* | *Ventura*
:---:|:---
##

## *Meu Setup*

*Config* | *Desktop*
:---:|:---
*Placa Mãe* | <a href="https://www.gigabyte.com/br/Motherboard/Z590-AORUS-PRO-AX-rev-10#kf" target="_blank">*Gigabyte Z590 AORUS PRO AX*</a>
*Gabinete* | *Fortress-tg Gamemax*
*Fonte* | *GIGABYTE - GP-P550*
*CPU* | *KV1K es (i9 11900K)*
*Water Cooler* | *DEEPCOOL GAMMAXX L120T*
*NVME M.2* | *XPG GAMMIX S11L 256GB / macOS*
*NVME M.2* | *XPG GAMMIX S41 512GB / Windows 11*
*GPU* | *RX 570 4G PowerColor*
*Memória ram* | *CORSAIR VENGEANCE LPX 2x16GB total 32GB*
*WI-FI / Bluetooth* | *AX200*
*Rede* | *Intel I225-V*
##

## *O que funciona*

- [x] *Áudio.*
- [x] *Rede.*
- [x] *WI-FI.*
- [x] *Bluetooth.*
- [x] *USB.*
- [x] *Sleep.*
##

## *Resultados Geekbench*
* _**Processador de engenharia KV1K es**_
  * *Por ser um processador de engenharia é necessário chave de ativação do [`Geekbench`](https://www.geekbench.com) para gerar os testes, eu não tenho!*

##

## *Captura de telas*

![sobre-mac](./img/about.png)
![som](./img/sound.png)
![internet](./img/network-wifi.png)
![bluetooth](./img/bluetooth.png)
![perifericos](./img/peripherals.png)
![versao-opencore](./img/opencore-version.png)
![kexts](./img/kexts.png)
![mapeamento-usb](./img/USB-mapping.png)
##

## *Kexts usadas, (todas versões Releases)*

- *[`WhateverGreen.kext`](https://github.com/acidanthera/WhateverGreen)*
- *[`Lilu.kext`](https://github.com/acidanthera/Lilu)*
- *[`VirtualSMC`](https://github.com/acidanthera/VirtualSMC), somente: `VirtualSMC.kext`, `SMCProcessor.kext` e `SMCSuperIO.kext`*.
- *[`AppleInteli210Ethernet.kext`](https://github.com/luchina-gabriel/youtube-files/raw/main/AppleIntelI210Ethernet.kext.zip)*
- *[`CpuTscSync.kext`](https://github.com/acidanthera/CpuTscSync)*
- *`USBMap.kext`*
- *[`AirportItlwm.kext`](https://github.com/OpenIntelWireless/itlwm/releases)*
- *[`BluetoolFixup.kext`](https://github.com/acidanthera/BrcmPatchRAM/releases)*
- *[`IntelBluetoothFirmware.kext`](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)*
- *[`ntelBTPatcher.kext`](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)*
##

## *Utilização*

* _**Recomendação 1**_
  * *Use [`GenSMBIOS`](https://github.com/corpnewt/GenSMBIOS), para gerar novos seriais para sua SMBIOS afim de evitar conflitos com iServices.*
* _**Recomendação 2**_
  * *Use [`ProperTree`](https://github.com/corpnewt/ProperTree), para editar seu config.plist.*     
* _**Recomendação 3**_
  * *Use [`USBMap`](https://github.com/corpnewt/USBMap), para mapear suas portas USB, apartir do OC 0.9.3, pode ser mapeadas com XHCIPortLimit habilitada no config.plist + [`USBInjectAll`](https://github.com/Sniki/OS-X-USB-Inject-All/releases).*
* _**Recomendação 4**_
  * *Extrair sua DSDT a partir do windows.*
  * *Use [`SSDTTime`](https://github.com/corpnewt/SSDTTime), para gera seus patches de SSDT.*    
* _**Recomendação 5**_
  * *Use [`MaciASL`](https://github.com/acidanthera/MaciASL), para compilar seus patches de SSDT.*
##

## *Configurações de BIOS Intel*

* _**Desativar**_

  * *Fast Boot*
  * *Secure Boot*
  * *Serial/COM Port*
  * *Parallel Port*
  * *VT-d (pode ser ativado se você definir DisableIoMapper como true)*
  * *Módulo de suporte de compatibilidade (CSM) (deve estar desativado na maioria dos casos, erros/paradas de GPU como gIO são comuns quando esta opção está ativada)*
  * *Thunderbolt (para instalação inicial, pois o Thunderbolt pode causar problemas se não for configurado corretamente)*
  * *Intel SGX*
  * *Intel Platform Trust*
  * *CFG Lock (proteção contra gravação MSR 0xE2) (deve estar desativado, se você não conseguir encontrar a opção, ative AppleXcpmCfgLock em Kernel -> Quirks. Seu hack não inicializará com o CFG-Lock ativado)*

* _**Habilitar**_

  * *VT-x*
  * *Above 4G Decoding (Resizable BAR -> Disable)*
  * *Hyper-Threading*
  * *Execute Disable Bit*
  * *EHCI/XHCI Hand-off*
  * *Tipo de SO: Modo UEFI do Windows 8.1/10 (algumas placas-mãe podem exigir "Outro sistema operacional")*
  * *DVMT pré-alocado (memória iGPU): 64 MB ou superior*
  * *Modo SATA: AHCI*
##

## *Agradecimentos*

- [*Acidanthera*](https://github.com/acidanthera)
- [*CorpNewt*](https://github.com/corpnewt)
- [*CrisHotpatch*](https://t.me/crishotpatch)
- [*Dortania*](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo)
- [*Dicas do Mateus*](https://www.youtube.com/c/DicasdoMateus)
- [*Gabriel Luchina*](https://www.youtube.com/c/gabrielluchina)
##

## *Licença* 

*The* [*MIT License*](./LICENSE.md) (*MIT*)

*Copyright :copyright: 2023* 
##
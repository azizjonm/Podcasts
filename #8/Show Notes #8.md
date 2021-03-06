[Noise Security Bit #8](http://noisebit.podster.fm/7)
=====
## О реверсинге firmware


### Участники:
Александр Матросов ([@matrosov](http://twitter.com/matrosov)),
Андрей Костин ([@costinandrei](https://twitter.com/costinandrei)),
Сергей Шекян ([@sshekyan](https://twitter.com/sshekyan)),
Александр Бажанюк ([@ABazhaniuk](http://twitter.com/ABazhaniuk))
Олег Купреев ([@090h](https://twitter.com/090h)),
Дмитрий Олексюк ([@d_olex](https://twitter.com/d_olex)),


###Инструменты для дампа SPI-flash памяти
* [Bus Pirate](http://dangerousprototypes.com/docs/Bus_Pirate)
* [GoodFET](http://goodfet.sourceforge.net)
* [DEDIPROG](http://www.dediprog.com/pd)

###Софт для дампа SPI-flash
* [CHIPSEC](https://github.com/chipsec/chipsec/blob/ac2ca7264f107c7b15ea8480db9c0e471dffd610/source/tool/chipsec/utilcmd/spi_cmd.py)
* [FlashROM](http://flashrom.org/Flashrom)

### Инструменты для реверсинга прошивок
* [Binwalk](http://binwalk.org/)

### Инструменты разработчика для BIOS/UEFI
* [Unified Extensible Firmware Specifications](http://www.uefi.org/specifications) - Спецификации на UEFI.
* [TianoCore](http://tianocore.github.io/) - OpenSource реализация UEFI и SDK.
* [EFI Toolkit](https://github.com/tianocore/tianocore.github.io/wiki/EFI-Toolkit) - Более старый, но при этом более простой в использовании UEFI SDK.
* [OVMF](http://tianocore.sourceforge.net/wiki/OVMF) - OpenSource реализация UEFI для виртуальных машин разрабатываемая в рамках TianoCore.
* [EFI Shell](https://github.com/tianocore/tianocore.github.io/wiki/Efi-shell) - Command line оболочка для UEFI.
* [Intel® AMT Software Development Kit](https://software.intel.com/en-us/articles/download-the-latest-intel-amt-software-development-kit-sdk)
* [Intel® Galileo](http://www.intel.com/content/www/us/en/do-it-yourself/galileo-maker-quark-board.html) - Development board от Intel, самый дешевый способ отлаживать UEFI на живом железе с использованием JTAG.
* [ARIUM - Intel and ARM JTAG Debuggers](https://www.arium.com/) - Более дорогой и продвинутый способ отлаживать UEFI на живом железе с использованием JTAG :)

### Инструменты для реверсинга BIOS/UEFI
* [CHIPSEC](https://github.com/chipsec/chipsec)
* [UEFI Firmware Parser](https://github.com/theopolis/uefi-firmware-parser) - Прим. от @d_olex: много багов и плохой код!
* [UEFITool](https://github.com/LongSoft/UEFITool) - Кросс-платформенная (Win/Linux/Mac) GUI программа для разбора и модификации UEFI образов. 
* [Flash Image Tool](https://dl.dropboxusercontent.com/u/22903093/Intel%20Flash%20Image%20Tool.zip) - Инструмент от Intel для конфигурирования различных параметров UEFI Flash Image, в архиве версии для чипсетов 6, 7 и 8 серий.
* [EFI scripts for IDA Pro](https://github.com/snare/ida-efiutils) - Дополнения для IDA облегчающие реверс-инжиниринг UEFI бинарников.
* [Copernicus](http://www.mitre.org/capabilities/cybersecurity/overview/cybersecurity-blog/copernicus-question-your-assumptions-about) - Инструмент от MITRE позволяющий (в теории) обнаруживать зловредные модификации BIOS.

### Уязвимости UEFI и атаки на SecureBoot
* [Summary of Attacks Against BIOS and Secure Boot](https://www.defcon.org/images/defcon-22/dc-22-presentations/Bulygin-Bazhaniul-Furtak-Loucaides/DEFCON-22-Bulygin-Bazhaniul-Furtak-Loucaides-Summary-of-attacks-against-BIOS.pdf)
* [Extreme Privilege Escalation On Windows 8/UEFI Systems](https://www.defcon.org/images/defcon-22/dc-22-presentations/Kallenberg/DEFCON-22-Corey-Kallenberg-Extreme-Privilage-Escalation-WP-UPDATED.pdf)

### Атаки на через USB
* [USB for all!](https://www.defcon.org/images/defcon-22/dc-22-presentations/Michael-Shkatov/DEFCON-22-Jesse-Michael-Mickey-Shkatov-USB-for-All!!-UPDATED.pdf)
* [Lessons learned from 50 bugs: Common USB driver vulnerabilities](https://www.nccgroup.com/media/190706/usb_driver_vulnerabilities_whitepaper_january_2013.pdf)
* [USB Fuzzing for the Masses](https://labs.mwrinfosecurity.com/blog/2011/07/14/usb-fuzzing-for-the-masses/)
* [Emulating USB Devices with Python](http://travisgoodspeed.blogspot.com/2012/07/emulating-usb-devices-with-python.html)

  ####Инструменты для анализа защищенности USB устройств
* [Facedancer](http://int3.cc/products/facedancer21)
* [Umap](https://github.com/nccgroup/umap)
* [GoodFET](https://github.com/travisgoodspeed/goodfet) - Facedancer firmware

### Foscam камеры и их клоны
* [GetMeCamTool](https://github.com/artemharutyunyan/getmecamtool) - Утилиты для pwnage и внедрения backdoor-a в удаленную камеру, сборщик/парсер прошивок для Foscam, сканер DynDNS сервиса Foscam
* [Заметки о Foscam камерах, уязвимостях в самих камерах и в DynNDS предоставляемый Foscam-ом](http://blog.shekyan.com/ip-camera/)

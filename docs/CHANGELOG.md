# CHANGELOG
All notable changes to this project will be documented in this file.  
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

> ### 2020-3-29
#### Added
SSDT-ALS0 hotpatch for faking ambient light sensor ALS0 per Catalina's brightness preservation.  
SSDT-GPRW hotpatching for fixing instant wake (0D/6D patch).  
#### Changed
SSDT-Keyboard with the exception of F7 and F12, now maps all hotkeys to a Fn value that can be remapped within macOS. In addition, PrtSc is now remapped to F13.
SSDT-PLNF to a cleaner version.
Similarly, battery patch has been simplified.
#### Removed
Some unused patches within OpenCore config.plist has now been removed.


> ### 2019-12-22
#### Added
Project website: https://tylernguyen.github.io/x1c6-hackintosh/  
ACPI dump for `BIOS-v1.43`.  
CHANGELOG.md to keep track of the project's developments.  
OpenCore bootloader, version `0.5.3`.  
Better SSDT patching with hotpatches under `patches`. Making sure to read `patches/README`.  
#### Changed
Switched completely to hotpatching through OpenCore. Credits to [daliansky](https://github.com/daliansky) and [jsassu20](https://github.com/jsassu20).  
Updated main README, made it look more visually appealing and organized.
#### Deprecated
Clover bootloader. Clover r5100 is the last version I used on this machine. Moving forward, OpenCore is my preferred bootloader. See `EFI-Clover/README.md`.  
Reorganized folder/project structure. Setup instructions and references now under `docs`.  
#### Removed
Old static patches.  
Old IORegistryExplorer dump.
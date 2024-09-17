# Opencore Acer Aspire E5-473

What's working : maybe basic stuff
What's doesn't working :
- sleep feature
- wifi & bluetooth
- microphone built-in detected, but doesn't work (speakers work fine)
- haven't add battery indicator and touchpad (because mine's broken)
- The display of opencore efi, is not showed at all (but still can interact with it) (this only happened on bigsur, when i installing from monterey is work fine) (also updated from bigsur to sonoma, still doesn't show up)

## How do i install it?
1. install Bigsur from Windows method (using macrecovery and LAN connection)
2. Disable SIP first from recovery
3. Download Opencore configurator and open it
4. From top bar, mount efi partition of internal disk, then copy that bigsur efi into it
5. Restart without usbdrive to see if it still work
6. Download OpencoreLegacyPatcher.app GUI and install it
7. Download macos update package from the Patcher app
8. Move efi-sonoma into usb drive, then restart into opencore of usb drive
9. If it doesn't boot, remove "amfi_get_out_of_my_way=1" first from boot-args of efi usb drive
10. When check about this mac, smbios changed into Macbook Air
11. Install macos update package manually in bigsur macos

## When installing update package, immediately add amfi_get_out_of_my_way=1 into boot-args of efi usb drive

12. Wait until it restart several times (2-3x)
13. After first boot into sonoma, open OpencoreLegacyPatcher app, and choose root patcher, it will patch graphics card, when finish popup appeared then restart
14. When everythings are done, copy efi-sonoma from efi usb drive into efi internal disk

## Device info
- Acer Aspire E5-473 (non-nvidia version)
- Intel I3-4005U @1.7Ghz
- RAM 8GB DDR3L 1600Mhz
- Intel HD 4400 (VRAM 1536MB Metal 2)
- SSD SATA VGEN 120GB
- Wifi card Broadcomm BCM43XXXA0

## Software Info
- OpenCore v1.0.0 DEBUG
- Updated to Sonoma (i think it could install Sequoia)

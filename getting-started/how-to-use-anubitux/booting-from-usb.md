# Booting from USB

When a computer is turned on, it usually runs the operating system installed on the main hard drive, like Windwos, Linux or MacOS.

Boot from USB device with a .iso file flashed on it may be different from device to device, depending on the manufacturer and on the configuration.

When using a **Mac device**, after the startup chime, it is necessary to press and hold the Option key to enter in the StartUp Manager and choose from which device the Operating System should be loaded.

With **other devices** there may be two solutions.

First of all, it may be possible to enter in the BIOS menu of the device and access the boot priority menu. In this menu it is necessary to give to the USB source an higher priority than to the internal hard drive. Doing so, every time the device is turned on with an USB drive flashed with a bootable .iso image, it will load the operating system written on it.

To enter in the BIOS menu, it is necessary to press a certain key repeatedly when the device is turned on, like **Esc**, **F1**, **F2**, **F8**, **F10** or **F12**. In some cases a message showing which key should be pressed is displayed for a few seconds before the boot process starts.

In other cases, repeatedly pressing the keys showed above, it is possible to enter in a dedicated menu where it is possible to choose from which source the user wants to get to operating system that should be loaded.

AnuBitux should work with both legacy and UEFI boots but In some cases, depending on the device, it may be necessary to set boot mode from one to another. It may also be necessary to disable the secure boot protection.

_<mark style="color:red;">Note that modern Windwos devices, with Bitlocker turned on, may ask for the recovery key after performing some modification to the BIOS menu, so it is heavily recomended to be sure to have access to it before trying any of the steps illustrated above.</mark>_

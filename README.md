# Acer-M5-583P Desktop Mojave 10.14 Hackintosh

This is tested on the Acer Aspire M5-583P-9688 but should work on any M5-583P variant. You will need to replace the wifi/bt chip with some that is compatible. Personally I have done it with the Broadcom BCM4352 Azurewave AW-CE123H, because it is a 2 antenna half sized card so it perfectly replaces the intel stock one.

## Hardware
* CPU - I7-4500U - 4th Gen
* Ram - 8gb - 2 slots
* GPU - Intel HD4400
* Drives - 2 AHCI/Sata SSD's
* Audio - Realtek UNKNOWN
* Ethernet - Realtek RTL8111 Series
* wifi/bt - Coming Soon

## Software
Used the [Vanilla guide](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/) and the [Internet Recovery install method](https://internet-install.gitbook.io/macos-internet-install/)

## Config.plist (Removed to protect my PC)
This is based on [RehabMan's HD4400 Base config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config/blob/master/config_HD4600_4400_4200.plist) with some minor changes like a generated SMBIOS.

* Requires Serial Number (ex. DFOWQLSGH8K)
* Requires Board-ID (ex. Mac-D859C5498DA9EE9D)

## Kext Explanation
TODO

## TODO
1. Install Broadcom BCM4352 Azurewave AW-CE123H WIFI/BT card when it arrives.
2. Map the USB Ports in the proper way instead of injecting them all.
3. Get the Battery and Charging being detected (Requires DSDT patching) It isn't the end of the world because the charging hardware will still work properly and the charging indicator led works as well.
4. Figure out what Realtek audio codec is being used so i can replace VoodooHDA with the proper AppleALC Kext.

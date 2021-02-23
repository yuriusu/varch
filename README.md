# Vanilla Arch Linux Installer

Reference implementation of the Arch Linux [Installation guide][1] written in Bash.

VArch is a simple Text-based User Interface (TUI) tool used to bootstrap a basic Arch Linux system.

## Usage

Download and execute the [script][0] (or run it directly) within a live environment:

```bash
bash -c "$(curl -L yuriusu.github.io/varch)"
```

> **Note:** Supports only UEFI boot mode and is limited to only ROOT, UEFI, and SWAP (or swapfile) partitions.

> **Note:** For beginners, consider reading the [wiki][1] first to get familiar with setting up an Arch Linux system.

Preparation            | Details
---------------------- | -----------------------------------------------------
List Block Devices     | Display currently attached block devices
[Partition Storage][2] | Secure wipe a device and/or modify partition layout
[Mount Partitions][3]  | Format and/or mount required partitions

Installation            | Details
----------------------- | ----------------------------------------------
[Update Mirrorlist][4]  | Change the mirror server list
[Install Packages][5]   | Installs the base and optional kernel packages

Configuration             | Details
------------------------- | --------------------------------------------------------
[Chroot Environment][12]  | Change root into the new system
[File Systems Table][6]   | Generates an FSTAB file
[Timezone and Clock][7]   | Sets the time zone and system clock
[Keyboard and Console][8] | Sets the keyboard layout and console font
[System Locale][8]        | Sets the default system locale
[Network Hostname][9]     | Sets the computer name on a network
[User Accounts][10]       | Add or remove a user as well as change a user's password
[System Bootloader][11]   | Installs recommended boot loader

[0]: https://yuriusu.github.io/varch
[1]: https://wiki.archlinux.org/index.php/Installation_guide
[2]: https://wiki.archlinux.org/index.php/Installation_guide#Partition_the_disks
[3]: https://wiki.archlinux.org/index.php/Installation_guide#Mount_the_file_systems
[4]: https://wiki.archlinux.org/index.php/Installation_guide#Select_the_mirrors
[5]: https://wiki.archlinux.org/index.php/Installation_guide#Install_essential_packages
[6]: https://wiki.archlinux.org/index.php/installation_guide#Chroot
[7]: https://wiki.archlinux.org/index.php/Installation_guide#Fstab
[8]: https://wiki.archlinux.org/index.php/Installation_guide#Time_zone
[9]: https://wiki.archlinux.org/index.php/Installation_guide#Localization
[10]: https://wiki.archlinux.org/index.php/Installation_guide#Network_configuration
[11]: https://wiki.archlinux.org/index.php/Installation_guide#Root_password
[12]: https://wiki.archlinux.org/index.php/Installation_guide#Boot_loader

# bootloaders

#For any bootloader(GRUB4DOS, GRUB, GRUB2, SYSLINUX)

#Installing grub i386-pc (MBR mode) from x86_64 pc needs following packages
apt-get install grub-pc-bin

#Command to mound partion Y of device sdX on /mnt
mount /dev/sdXY /mnt

#Command to install grub i386-pc (MBR mode) on device sdX
grub-install --no-floppy --target=i386-pc --boot-directory=/mnt/boot/ /dev/sdX

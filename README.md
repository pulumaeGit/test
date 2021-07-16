Using dfu-util 
Flashing a .dfu file to the device:
$ dfu-util -a 0 -D boot_image.dfu

Reading out 1 KB of flash starting at address 0x8000000:
$ dfu-util -a 0 -s 0x08000000:1024 -U newfile.bin

Flashing a binary file to address 0x8004000 of device memory and ask the device to leave DFU mode:
$ dfu-util -a 0 -s 0x08004000:leave -D imagefile.bin

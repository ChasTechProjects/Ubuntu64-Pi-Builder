u-boot binaries that are compatible with the Raspberry Pi 3 and 4.

You must choose which one you want to use before building. The binaries are currently not cross-compatible, so you can't run RPi 3 u-boot on the RPi 4 or vice versa,

To choose find this line in the stage 1 script:

 <code>sudo cp u-boot/u-boot_rpi3.bin /mnt/boot/firmware/kernel8.img</code>
 
 And replace 'u-boot_rpi3.bin' with 'u-boot_rpi4.bin' if building for the Raspberry Pi 4, but if building for the Pi 3 then just leave it.
 
 If you plan on publicly distributing your built Ubuntu image then it's best to tell your users how to swap the u-boot binaries with the one compatible with their model.
 
 

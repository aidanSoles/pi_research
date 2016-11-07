Contributors:
  Aidan Daniels-Soles
  Gabriel Dalton
To compile for the Raspberry Pi 2 Model B:
arm-none-eabi-gcc -O2 -mfpu=vfp -mfloat-abi=hard -march=armv6zk -mtune=arm1176jzf-s -nostartfiles main.c -o kernel.elf && arm-none-eabi-objcopy kernel.elf -O binary kernel.img

Then add kernel.img, bootcode.bin, start.elf on your sd card and put it into your RPI and plug it into its power source!

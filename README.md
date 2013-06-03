# APC Uboot and Kernel


## u-boot

     export PATH=$PATH:$arm-toolchain/bin
     cd u-boot
     make wmt_config
     make all
     
## Kernel

     // on debian
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make oldconfig
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make menuconfig
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- INSTALL_MOD_PATH=$.modules make modules_install
     make ubin CROSS_COMPILE=arm-linux-gnueabi-






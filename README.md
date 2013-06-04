# APCKernel build

## Kernel

     // on debian squeeze
     add : deb http://www.emdebian.org/debian squeeze main to /etc/apt/sources.list
     aptitude update
     aptitude install gcc-4.4-arm-linux-gnueabi gcc-4.4-arm-linux-gnueabi-base
     cd kernel
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make oldconfig
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make menuconfig
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make ubin
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- make modules
     ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- INSTALL_MOD_PATH=./modules make modules_install







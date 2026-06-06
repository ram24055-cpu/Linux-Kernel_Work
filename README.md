# Linux-Kernel_Work
This is first linux kernel work repo, to learn Linux Kenel concepts.
<br>
Author - Ramdas Karhale
Step1 - Download latest kernel code from https://kernel.org
        I have downloaded linux-7.0.11.tar.xz
        Extract using - tar -xvf linux-7.0.11.tar.xz
        cd linux-7.0.11
        --------------------------------------------------
        Configure kernelfor ARM
        make ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- vexpress_defconfig
        Build kernel image and DTB
        make ARCH=arm CROSS_COMPILE=arm-linux-gnueabi- zImage dtbs -j$(nproc)

        ls -l arch/arm/boot/zImage
        ls -l arch/arm/boot/dts/arm/vexpress-v2p-ca9.dtb

        

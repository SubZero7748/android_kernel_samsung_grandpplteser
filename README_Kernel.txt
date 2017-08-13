################################################################################

1. How to Build
	- get Toolchain
		From android git server , codesourcery and etc ..
		 - Ex ) arm-eabi-4.8 or arm-linux-androideabi-4.9
		
	- edit Makefile (or using make option)
		edit "CROSS_COMPILE" to right toolchain path(You downloaded).
		  EX)  CROSS_COMPILE= $(android platform directory you download)/android/prebuilts/gcc/linux-x86/arm/arm-eabi-4.8/bin/arm-eabi-
		  Ex)  CROSS_COMPILE=/usr/toolchains/gcc/linux-x86/arm/arm-eabi-4.8/bin/arm-eabi-          // check the location of toolchain
  	
		$ make ARCH=arm mt6737t-grandpplte_defconfig
		$ make ARCH=arm

2. Output files
	- Kernel : arch/arm/boot/zImage
	
3. How to Clean	
		$ make clean
		$ make ARCH=arm distclean
################################################################################

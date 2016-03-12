# android_samsung_sm-g355h_kernel
  Linux kernel release 3.x <http://kernel.org/>

1. How to Build Kernel:
	First navigate to your kernel source folder. In my case:

		cd /home/darkside/android/kernel/samsung/kanas3gxx
		
	Than set path to your toolchain. In my case:
	
		export PATH=$PATH:/home/darkside/android/prebuilts/gcc/linux-x86/arm/arm-eabi-4.6/bin
		
	Than set arch and arm:
	
		export ARCH=arm
		export SUBARCH=arm
		export CROSS_COMPILE=arm-eabi-
		make kanas3g_hw04_defconfig
		make
		
	Your kernel will be in my case in:
	/home/darkside/android/kernel/samsung/kanas3gxx/arch/arm/boot (image = uncommpresed kernel zImage = commpresed kernel
	
	
2. Allways before new build make clean:

		make mrproper
		
    
3. Kernel has enabled IO Schedulers and CPU Frequency scaling

email:microzans@gmail.com         
Thanks Y300-0100

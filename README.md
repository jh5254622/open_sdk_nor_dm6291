norflash boot+8801 wifi
编译固件：
    直接make，如果要配置，则make menuconfig配置应用，make kernel_menuconfig配置kernel；
固件生成的bin位于bin\xburst目录中，6291-nor-16MB.bin是烧录固件，6291-nor-update-fw.bin是升级文件

uboot位于目录uboot\u-boot-dm6291-new-nor中
编译：
首次编译需要执行：make canna_v10_uImage_sfc_nor生成配置，后面直接make就行
u-boot-with-spl.bin是生成的uboot；copy到uboot目录下，重命名成uboot-6291-norboot.bin，编译固件时会自动打包到烧录文件中去。

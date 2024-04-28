# hexabitz-u-boot-v2023-04

# Download repository
    git clone https://github.com/hexabitz/hexabitz-u-boot-v2023-04.git
    cd hexabitz-u-boot-v2023-04
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make imx93_hexabitz_config
    make
    cp u-boot.imx /tftp/uboot-imx93.imx

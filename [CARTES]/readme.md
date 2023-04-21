Ici git *

## SPI
https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/Documentation/spi/spi-summary?h=v4.19.78
https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/Documentation/spi/spidev?h=v4.19.78
https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/arch/arm/boot/dts/at91-sama5d27_som1_ek.dts?h=v4.19.78

## GPIOS
https://www.kernel.org/doc/Documentation/gpio/gpio.txt

### I2c-tools

    apt-get install i2c-tools

### MPIO

    sudo apt install python3-pip
    pip install mpio
    
### Gpiod

    sudo apt install gpiod
    
### Gpios sur python

    sudo apt install python3-libgpiod
    
### Dougg Gilbert GPIO utils (casser sur Armbian)

    sudo apt install xz-utils build-essential
    wget https://www.acmesystems.it/www/dougg_gilbert_gpio_utils/sama5d3_utils-0.92.tar.xz
    tar -xvf sama5d3_utils-0.92.tar.xz
    Compile and install
    cd sama5d3_utils-0.92
    make
    sudo make install
    
#

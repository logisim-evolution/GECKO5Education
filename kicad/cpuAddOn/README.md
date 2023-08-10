# GECKO5Education CPU-addon

This design can be used with the GECKO5Education or standalone and provides
an educational base for programming related classes.
In case this board is used with the GECKO5Education, the FTDI-chip is automatically
routed to the integrated USB-hub, meaning that you only require one USB-C connection. 
In case of this situation, the USB-C connector of the GECKO5Education is disabled, and all
functionality is provided by the USB-C connector of the CPU-addon board.

# Debugging

This board integrates a [Black Magic Probe](https://black-magic.org/index.html). After production
it needs to be programmed with the DFU-firmware once by an external programmer. After this firmware-
updates can be performed as with the normal Black Magic Probe.

# External connections

This boards integrates an extention connector (32 positions) that provides two 
[PMOD-compatible](https://digilent.com/reference/_media/reference/pmod/pmod-interface-specification-1_2_0.pdf)
interfaces. The different possibilities are listed below:

PMOD1:

|Pin|function1|function2|function3|
|:-:|:--------|:--------|:--------|
|1  |GPIO     |SPI6nCS  |I2S1_WS  |
|2  |GPIO     |SPI6MOSI |I2S1_SDO |
|3  |GPIO     |SPI6MISO |I2S1_SDI |
|4  |GPIO     |SPI6SCK  |I2S1_CK  |
|7  |GPIO     |EXTI5    |         |
|8  |GPIO     |EXTI6    |         |
|9  |GPIO     |SCL4     |         |
|10 |GPIO     |SDA4     |         |

PMOD2:

|Pin|function1|function2|function3|
|:-:|:--------|:--------|:--------|
|1  |GPIO     |CTS2     |         |
|2  |GPIO     |TX2      |         |
|3  |GPIO     |RX2      |         |
|4  |GPIO     |RTS2     |         |
|7  |GPIO     |EXTI13   |         |
|8  |GPIO     |ADC1_2_3 |EXTI0    |
|9  |GPIO     |ADC1_2_3 |EXTI1    |
|10 |GPIO     |ADC3     |EXTI10   |


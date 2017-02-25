# avr_integration

This local project is for AtMega328P

The main purpose is to use 328P for reading analog values and pushing data to MAX7219 drivers.
This is required because of only one ADC channel on nodeMCU. Also, to nodeMCU will be connected a SD-card, which will use the one available SPI lines.
AtMega328P will provide additional SPI channel for MAX7219.

Communication between nodeMCU and Atmega328P will be done using UART(?) or I2C(?)

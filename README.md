# avr_integration

This local project is for AtMega328P

The main purpose is to use 328P for reading analog values and pushing data to MAX7219 drivers.
This is required because of only one ADC channel on nodeMCU. Also, to nodeMCU will be connected a SD-card, which will use the one available SPI lines.
AtMega328P will provide additional SPI channel for MAX7219.

Communication between nodeMCU and Atmega328P will be done using UART(?) or I2C(?)

Measurements should be performed by timer, initiated by nodeMCU side. AtMega328P waits for incoming request and, after it's analizing, perform required measurements and return results.

Sent data will consists of:
- temperature values in format %2f
- humidity in format dd
- solar panel voltage in format %2f

Received data:
-...

SoftI2cMaster
=============

Arduino Library required to change I2C address of MCP4728 LDAC

The latch pin on the MCP4728 (12-Bit, Quad Digital-to-Analog Converter with EEPROM Memory) requires very specific timing to change the I2C address.
That timing cannot be generated using the Arduino Wire library. This library implements that timing by bit-banging the Arduino I2C pins and does not use the Arduino I2C hardware.

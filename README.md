# esp8266-sensactio
Repository for ESP8266 interface code for SensAct.IO

## Project Goal
This module shall fulfil all the requirements for a properly configured ESP8266 to connect to the SensAct.IO platform.

## Setup
### Important Settings
[TBD]

### Electronic Requirements
The attached device should be a ESP8266 chip.
Confirm hookup is as follows:
- VCC to 3.3V, GND to Ground
- 3.3V via Resistors on GPIO0, GPIO2, GPIO15
- Attach CH_PD to ground to reset
- Attach GPIO0 to ground to allow programming


One or two BMP280 chips should be connected via GPIO4 and GPIO5. 
 - Note: If the CSB lead is grounded on a BMP280 then the I2C address 'might' change to 0x76 (from it's default of 0x76). 
         I say 'might' because according to some notes online - this change of address may not apply to all chips
 
### Test Process
Before starting - ensure the ESP8266 is known to successfully run a 'blink' type program with a LED on IO13 (I.e. not somehow fried). 
- BMP280 should return appropriately formatted result when data is requested 
- 

# TOF Sensor Board
# Requirements
- CAN FD support at minimum 5 Mbps
- Small overall footprint
- Multiple connectors for daisy-chaining
# Component selection
- ## Sensors:
	### VL53L8CX:
	- [$8.01000](https://www.digikey.com/en/products/detail/stmicroelectronics/VL53L8CXV0GC-1/18085238)
	- Modern ST sensor
	- 64 point TOF measurement
	- Up to 4m range
	- SPI interface at 3MHz
	- Requires 3.3V and 1.8V rails
- ## MCU
	### STM32G0B1CCU7:
	- [$2.798](https://www.lcsc.com/product-detail/C29759424.html?s_z=n_q_C29759424&globalKeyword=C29759424)
- ## Communication:
	### 74AVC4T774GUX:
	- [$0.6337](https://www.lcsc.com/product-detail/Translators--Level-Shifters_Nexperia-74AVC4T774GUX_C546275.html)
	- Used to convert 1.8V SPI from the sensor to 3.3V SPI for the MCU
	### TCAN3403DDFRQ1:
	 - [$1.6007](https://www.lcsc.com/product-detail/C35926232.html?globalKeyword=C35926232&s_z=n_q_C35926232)
	 -  CAN FD Transceiver supporting up to 5Mbps
	 - Runs off 3.3V with no 5V requirement

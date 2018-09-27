# Arduino-GPS
## This task was to build a node that could use a GPS module to get it's current location from a satellite. It would then send it's location over the LoRaWAN. Using a web app we can then visually display the strength of the connection on a map of Dunedin. This will help us map out the city, so we know what areas are able to connect to LoRa, and which aren't. This helps us know the range of our network, and where we need to put more gateways. 

### Preparation
	Preparation for this node is fairly simple. The only things required are the Arduino IDE and the suitable drivers. 
	
## Required Hardware

- Arduino board
- Breadboard
- Battery pack
- Arduino LoRa shield
- NEO-6M-0-001 GPS Module
- LED's
- Resistors
- Wires

## Wiring

Using the corresponding Arduino pins on the UDK

![Wiring diagram](resources/GPSwiring.jpg "Wiring diagram")

### Wiring standard:

Red wires should only be used for voltage.

Black wires should only be used for ground.

Wires of other colors can be used to connect pins to analog or digital. 

### Wiring guide for GPS Module:
	NEO-6M GPS Module:		Wiring to Arduino UNO:
	VCC						5V
	RX						TX pin defined in the software serial
	TX						RX pin defined in the software serial
	GND						GND
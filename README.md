ISOLATED_POWER_SUPPLY_BOARD
This repository contains the complete design files for an isolated multi-voltage power supply PCB developed for embedded systems, IoT products, and electronics prototyping
### Isolated Multi-Voltage Power Supply Board

This repository contains the complete design files for an isolated multi-voltage power supply PCB intended for embedded systems, IoT hardware, and general electronics prototyping where **electrical safety, noise isolation, and power-domain separation** are critical.

The board is designed around a 230VAC mains input and converts it into low-voltage isolated DC rails, while also supporting an independent external DC input. The isolation ensures that the low-voltage logic side remains electrically separated from the high-voltage mains side, significantly improving user safety and system reliability.

Power Architecture

The board provides multiple regulated voltage areas, each intentionally separated:

* Isolated 5V DC rail for microcontrollers, USB devices, and digital peripherals
* Isolated 3.3V DC rail for low-power MCUs, sensors, and communication modules
* Auxiliary VIN input (0–12V DC) through a DC jack or external adapter allowing the board to operate without mains power when required
* USB-C breakout supply path powered from the regulated 5V rail, enabling easy connection to development boards and external modules

Each voltage domain is routed in a dedicated section of the PCB to minimize coupling, noise, and accidental shorting between power rails.

### Safety & Design Considerations

Special attention has been given to high-voltage PCB layout practices:

* Clear primary and secondary isolation zones
* Proper creepage and clearance spacing between mains and low-voltage areas
* Provision for **fuse protection, MOV, and EMI suppression components
* Thoughtful connector placement to prevent misuse or unsafe wiring

The layout is intended to be **manufacturable, inspectable, and serviceable**, rather than a conceptual or academic design.

Intended Use

This board can act as a central isolated power hub for:

* Embedded controller boards
* Sensor and communication modules
* USB-powered devices
* Prototyping and lab setups requiring safe mains isolation

Repository Contents

* Schematic design files
* PCB layout files
* 3D PCB renders
* Documentation and usage notes

This project focuses on practical power electronics design emphasizing safety, clarity, and real-world usability over shortcuts or minimal designs.

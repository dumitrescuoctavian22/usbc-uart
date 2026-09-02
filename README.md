USB-C → UART Adapter

A compact USB-C to UART adapter designed around the CP2102 USB-to-UART bridge. The board provides a simple interface for connecting a computer to microcontrollers and other embedded systems through a standard UART interface.

The PCB was designed from schematic to layout in KiCad as a 2-layer board, with USB 2.0 connectivity, ESD protection, status LEDs, and an accessible UART header.

Features

- USB-C input
- CP2102 USB-to-UART bridge
- USB 2.0 interface
- USB ESD protection using ST USBLC6-2SC6
- 5-pin UART header
- Power and UART activity indicators
- 2-layer PCB
- Designed in KiCad

UART Header

The UART interface is exposed through a 5-pin header:

Pin| Function
1| RX

2| TX

3| 3V3

4| 5V

5| GND

USB-C Interface

The board uses a 16-pin USB-C receptacle for USB 2.0 communication.

The USB interface includes the USB data lines, power connections, and USB-C configuration connections. ESD protection is provided by the ST USBLC6-2SC6, protecting the USB data interface against electrostatic discharge.

USB-to-UART Conversion

The CP2102 is the main USB-to-UART bridge on the board.

It handles the conversion between USB communication from the host computer and the UART interface exposed on the header.

The board is intended to provide a convenient interface for development, debugging, and communication with embedded systems.

Status LEDs

Three LEDs are included on the board:

LED  | Color | Function

Power| Green | Power indication

RX   | Red   | UART receive activity

TX   | Yellow| UART transmit activity


These indicators provide visual feedback for power and UART communication.

PCB Design

The PCB was designed as a 2-layer board in KiCad.

The design process included:

- Schematic capture
- Component selection
- USB-C interface design
- USB ESD protection
- CP2102 USB-to-UART implementation
- Component placement
- PCB routing
- Power distribution
- UART header layout
- 3D PCB visualization

Particular attention was given to keeping the USB interface compact and placing the ESD protection around the USB connection.

Repository Structure

usbc-uart/

├── README.md

├── documentation/

├── hardware/

├── images/

└── manufacturing/

The repository contains the KiCad hardware design files, documentation, images, and manufacturing-related files.

Tools

- KiCad — schematic and PCB design
- KiCad 3D Viewer — PCB visualization

Project Status

PCB designed — not yet manufactured or tested.

This project currently represents the completed PCB design and serves as a practical demonstration of USB-C interfacing, USB-to-UART conversion, ESD protection, component placement, and 2-layer PCB routing.

What I Learned

This project was created to develop practical PCB design skills while working with a real USB interface and USB-to-UART bridge.

The main areas explored were:

- USB-C connector implementation
- USB 2.0 interface design
- USB ESD protection
- CP2102 integration
- UART interface design
- Power distribution
- PCB component placement
- 2-layer PCB routing
- KiCad schematic-to-PCB workflow
- PCB documentation and organization
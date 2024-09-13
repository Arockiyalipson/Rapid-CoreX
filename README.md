# Rapid_CoreX (Under Development)

![KiCad](https://img.shields.io/badge/Tool-KiCad-blue?logo=kicad)
![STM32CubeMX](https://img.shields.io/badge/Tool-STM32CubeMX-brightgreen?logo=stmicroelectronics)
![License: MIT](https://img.shields.io/badge/License-MIT-green)

## Introduction

Rapid-CoreX is a versatile Electronic Control Unit (ECU) designed for embedded systems development, testing, and integration. It supports essential communication protocols and allows for easy connection and testing of various sensors or devices using MATLAB software. Rapid-CoreX is particularly useful for testing external parameters of Battery Management Systems (BMS), motor controllers, and other connected devices.

## Tools Used

- **KiCad:** Used for schematic capture and PCB layout design.
- **STM32CubeMX:** Used for setting up the pin map for the design

## Design Structure

```bash
Rapid-CoreX
        │   LICENSE
        │   README.md
        │
        ├───Design
        │       Communication_interface.kicad_sch
        │       Rapid_Core-RCP.kicad_pcb
        │       Rapid_Core-RCP.kicad_pro
        │       Rapid_Core-RCP.kicad_sch
        │
        ├───Images
        │       Image.txt
        │
        ├───Manufacturing_files
        │   ├───Bom file
        │   │       BOM.txt
        │   │
        │   ├───Component position files
        │   │       Comp_pos.txt
        │   │
        │   ├───Drill files
        │   │       Drill.txt
        │   │
        │   ├───Gerber files
        │   │       Gerber.txt
        │   │
        │   └───Reference_material
        │           PDF.txt
        │
        └───Reference
                Application_note_for_STM32F4_family.pdf
                Common_mode_choke_less_CAN_BUS.pdf
                ISO1042-Q1_ISO_CAN_Datasheet.pdf
                ISO_3088_RS-485_ISO.pdf
                Reference_mannual_STM32F446xx.pdf
                Reference.ioc
                RS-485_Design_guide.pdf
                stm32f446xx_Data_Sheet.pdf
```

## Features

### Communication Protocols

Rapid-CoreX includes the following communication protocols for sensor connection, data collection, and interconnection:

#### Basic Protocols

- **SPI**: Serial Peripheral Interface for high-speed communication.
- **I2C**: Inter-Integrated Circuit for connecting multiple sensors.
- **UART**: Universal Asynchronous Receiver-Transmitter for serial communication.

#### Debugging

- **SWD**: Serial Wire Debug for in-circuit debugging and programming.

#### Data Collection and Interconnection Protocols

- **CAN**: Controller Area Network for real-time data exchange in automotive and industrial applications.
- **RS-485**: A robust standard for long-distance communication.
- **LIN**: Local Interconnect Network, used in automotive networks for communication between components.

All data collection protocols are isolated to ensure better protection and signal integrity.

### Communication Ports

Rapid-CoreX is equipped with various ports to facilitate connectivity:

- **2 x CAN** ports for network communication.
- **2 x RS-485** ports (USART) for long-distance and robust communication.
- **2 x LIN** ports for automotive applications.
- **2 x External SPI** ports for additional SPI device connectivity.
- **2 x I2C** ports for connecting multiple sensors or devices.
- **1 x I2C** with integrated SHT30 sensor for humidity and temperature measurement.

### GPIO Features

- **User LED**: Available for user-defined visual indication.

## Applications

Rapid-CoreX is ideal for:

- Testing external parameters of Battery Management Systems (BMS).
- Testing motor controllers.
- Integrating and testing various sensors.
- Development and testing of embedded systems that require robust and isolated communication.

## Getting Started

### Prerequisites

To use Rapid-CoreX, ensure you have the following:

- MATLAB software for interfacing and testing.
- Necessary drivers and libraries for STM32 Cortex-M4.

### Setup

1. Connect your sensors or sister devices to the appropriate communication ports on Rapid-CoreX.
2. Use MATLAB to interface with Rapid-CoreX for data collection and testing.
3. For debugging, connect through the SWD interface.

### Usage

1. Power on the Rapid-CoreX and ensure all connections are secure.
2. Implement a MATLAB Developed Algorithm in the board
3. Start collecting Data and Analyze it 


## Contact

For more information, please contact [Arockiya Lipson](https://www.linkedin.com/in/arockiya-lipson-458b12214).


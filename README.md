# STM32 Development Board V1.1

A professional development board based on the **STM32G431VBT6** microcontroller, featuring multiple GPIO options, dual USB-C connectors, and dual crystal oscillators for precision timing applications.

## Overview

This development board is designed as a versatile platform for embedded systems development, IoT applications, and microcontroller prototyping. The STM32G431VBT6 is a powerful ARM Cortex-M4 processor running at up to 170 MHz.

## Key Features

### Microcontroller
- **Processor**: STM32G431VBT6 (ARM Cortex-M4)
- **Clock Speed**: Up to 170 MHz
- **Flash Memory**: 256 KB
- **RAM**: 36 KB
- **Package**: LQFP100

### Connectivity & Power
- **Dual USB-C Connectors** - Multiple connectivity options and power delivery
- **Multiple GPIO Pins** - Extended I/O options for sensors and peripherals (80 total pins)
- **Dual Crystal Oscillators** - Precision timing and redundancy support

### Physical Design
- **GPIO Layout**: Organized left and right side connectors for easy access
- **Mounting**: Four mounting holes for secure installation
- **PCB Layers**: 4-layer design for optimal signal integrity

## Pin Configuration

The board features **80 GPIO pins** arranged as follows:
- **40 pins per side** (Left and Right)
- **Clearly labeled for easy identification**
- **Support for analog and digital functions**

## Applications

- IoT Devices - Connected sensors and remote monitoring
- Robotics - Motor control and sensor integration
- Data Acquisition - Multi-channel ADC and timing-critical applications
- Prototyping - Rapid embedded systems development
- Power Management - Efficient DC-DC conversion and power delivery

## Getting Started

### Required Tools
- STM32CubeIDE or ARM MDK
- ST-LINK V2 Debugger (or compatible)
- USB-C Cable
- Appropriate ST firmware libraries

### Basic Setup
1. Connect ST-LINK debugger to the board
2. Connect USB-C for power and communication
3. Flash your firmware using STM32CubeProgrammer
4. Start developing!

## Documentation

| Resource | Link |
|----------|------|
| **Microcontroller Datasheet** | [STM32G431 Datasheet](https://www.st.com/resource/en/datasheet/stm32g431vb.pdf) |
| **Development Environment** | [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) |
| **Programmer Tool** | [STM32CubeProgrammer](https://www.st.com/en/development-tools/stm32cubeprog.html) |

## Hardware Specifications

| Specification | Value |
|---------------|-------|
| **Core** | ARM Cortex-M4 |
| **Clock Speed** | 170 MHz |
| **Flash Memory** | 256 KB |
| **SRAM** | 36 KB |
| **GPIO Pins** | 80 |
| **ADC Channels** | Multiple |
| **Timers** | Multiple (16/32-bit) |
| **UART/USART** | Multiple |
| **SPI/I2C** | Multiple |
| **USB** | 2x USB-C |
| **Crystals** | 2x (Dual oscillator support) |

## Repository Structure

```
STM32_DEVBOARD_V1.1/
├── README.md
├── Hardware/
│   ├── README.md
│   ├── PCB/
│   │   ├── STM32_DEVBOARD.PcbDoc
│   │   ├── STM32_DEVBOARD.SchDoc
│   │   └── Gerbers.zip
│   └── Schematics/
│       └── STM32_DEVBOARD_Schematic.pdf
└── Images/
    ├── Capture d'écran 2026-06-03 210806.png
    ├── Capture d'écran 2026-06-03 210849.png
    └── Capture d'écran 2026-06-03 211053.png
```

## Project Status

- ✅ PCB Design Complete
- ✅ Layout Verification Done
- 🔄 Manufacturing Phase
- ⏳ Testing & Validation (Coming Soon)

## License

This project is licensed under the [MIT License](LICENSE) - free to use, modify, and distribute.

## Contact & Support

**Author**: Felix-JRDB  
**Email**: felixjeanrichard4@gmail.com  
**Repository**: https://github.com/Felix-JRDB/STM32_DEVBOARD_V1.1

For issues, suggestions, or contributions, please open an issue on GitHub.

---

**Last Updated**: June 2026  
**Version**: 1.1

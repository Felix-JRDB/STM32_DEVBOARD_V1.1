# Hardware Documentation

This directory contains the Altium hardware design files for the STM32 Development Board V1.1.

## Contents

- **PCB/** - PCB design files and Gerber outputs
  - `STM32_DEVBOARD.PcbDoc` - PCB layout file
  - `STM32_DEVBOARD.SchDoc` - Schematic file
  - `Gerbers.zip` - Manufacturing-ready Gerber files

## Design Files

The design files are in Altium Designer format. To view or edit these files, you need:
- Altium Designer 21.0 or later, or
- Free Altium viewer for viewing only

## PCB Specifications

- **Layer Count**: 4 layers
- **Board Size**: Optimized for standard prototyping
- **Component Density**: Medium
- **Target Manufacturer**: Standard PCB fabrication

## Gerber Files

The `Gerbers.zip` file contains all necessary layers for PCB manufacturing:
- Top copper layer
- Bottom copper layer
- Internal layers
- Solder mask layers
- Silkscreen layers
- Drill files

## Manufacturing Notes

When ordering PCBs, use the Gerber files with these specifications:
- Board thickness: 1.6mm
- Copper weight: 1oz (35µm)
- Surface finish: HASL or ENIG recommended
- Solder mask color: Green (standard)

For more information, refer to the main [README.md](../README.md).

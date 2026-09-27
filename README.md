# AG32VF407

English reference material and examples for the AGM AG32VF407 RISC-V microcontroller family.

## Overview

The AG32VF407 is a RISC-V microcontroller with integrated programmable logic resources. This repository contains reference material, hardware-related resources, and example projects for both the MCU and AGRV2K programmable-logic functions.

## Key features

- RISC-V RV32IMAFC core, up to 248 MHz
- 128 KB SRAM with 512 KB or 1 MB Flash options
- Three 12-bit ADCs, up to 3 Msps in triple-interleaved operation
- Two 10-bit DACs and two comparators
- AGRV2K programmable logic device
- CAN 2.0, five UARTs, two I2C controllers, SPI, RTC, SDIO, and Ethernet MAC
- USB full-speed and OTG support
- Five advanced timers and two basic timers

The AG32VH407RCT6 variant includes 8 MB pSRAM with a claimed maximum access rate of 200 MB/s. Confirm part-specific limits, package options, and pin assignments in the vendor documentation before selecting a device.

## Repository layout

| Path | Contents |
| --- | --- |
| `src/` | Reference source code and example projects |
| `docs/` | Device and development documentation |
| `project/` | Project resources and reference designs, where provided |

## Development environment

- Develop the MCU software with VS Code and the supplied toolchain packages.
- Develop CPLD or FPGA logic with Quartus-compatible Verilog flows, then synthesize with the required Supra tooling.
- Supported programming and debugging options include J-Link V9 or later, AGM BLASTER, and CMSIS-DAP.

Review the selected board's power, clock, GPIO, and debugger configuration before programming hardware.

## License

This repository retains the included [MIT License](LICENSE). Keep the license and copyright notices when redistributing the material.

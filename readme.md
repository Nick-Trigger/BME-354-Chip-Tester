# BME 354 Chip Tester

A custom PCB designed to test analog ICs — specifically the ADC623 and INA126 instrumentation amplifiers — as part of a BME 354 course project.

## Overview

The board provides:

- A sine wave generator signal source
- A regulated voltage supply
- LED indicators for pass/fail output comparison
- Switch-controlled power and signal routing
- Test points for oscilloscope / multimeter probing

## Project Files

| Folder / File | Description |
| --- | --- |
| [KiCad_milling_machine/](KiCad_milling_machine/) | KiCad schematic and PCB layout files (milling-machine spec) |
| [KiCad_milling_machine/Custom Libraries/](KiCad_milling_machine/Custom%20Libraries/) | Custom KiCad symbols and footprints for non-standard parts |
| [Documentation/](Documentation/) | Photos from build and testing stages |
| [Documentation.md](Documentation.md) | Full design log with dated entries and schematic notes |

## Key Schematics

- [ChipTester_354.kicad_sch](KiCad_milling_machine/ChipTester_354.kicad_sch) — top-level schematic
- [AD_INA.kicad_sch](KiCad_milling_machine/AD_INA.kicad_sch) — ADC623 / INA126 test circuit
- [wave_generator.kicad_sch](KiCad_milling_machine/wave_generator.kicad_sch) — sine wave generator sub-circuit
- [pwrsup.kicad_sch](KiCad_milling_machine/pwrsup.kicad_sch) — voltage regulator sub-circuit
- [mcp_if.kicad_sch](KiCad_milling_machine/mcp_if.kicad_sch) — MCP interface sub-circuit

## Design Log

See [Documentation.md](Documentation.md) for a full chronological record of design decisions, breadboard testing, PCB layout, milling, soldering, and troubleshooting.

## Components

Non-standard parts sourced from DigiKey. Custom footprints included in [KiCad_milling_machine/Custom Libraries/](KiCad_milling_machine/Custom%20Libraries/) for:

- `100DP1T2B4M6QE` — DPDT slide switch
- `100SP3T2B4M6RE` — SP3T slide switch
- `7101MD9AQE` — rotary switch
- `BH9VPC` — 9V battery holder
- `PRS12R_4025K_103B1` — potentiometer

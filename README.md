# CommCase

> A proof of concept for a 3D-printable, modular emergency communications kit with interchangeable components

## Overview

This project provides a modular framework for building emergency communications (EMCOMM) go-kits that can be easily customized and reconfigured without fabrication of new parts. The system uses 3D-printed structural components, module enclosures, and panel-mounted equipment to create a flexible communications platform that fits inside protective cases like Pelican cases.

**Key Features:**
- **Modular Design** - Swap equipment without redesigning the entire panel
- **Case Agnostic** - Move layouts between different case sizes with minimal work
- **Non-Destructive** - No drilling or permanent modifications to cases
- **Interoperable** - Uses Powerpole connectors and standard dimensions for compatibility

## Project Structure

```
.
├── cad/              # FreeCAD source files
├── stl/              # Ready-to-print STL files
│   ├── Borders/      # Case-specific border components
│   ├── Modules/      # Equipment module enclosures
│   └── Structure/    # Rails, connectors, and mounts
└── README.md
```

## Guide

An assembly guide and video will be published soon.


## Design Principles

This system follows several key design guidelines:

- **External Power** - Uses external 12V power via Powerpole connectors (not internal batteries)
- **Powerpole Standard** - All 12V connections use Powerpole in RRTT orientation (Red-Right, Tongue-Top)
- **Standard Dimensions** - Modules are 100mm wide (or 50mm for center panels), heights in 50mm increments
- **3mm Top Panels** - Ensures consistent mounting across modules
- **Friction-Fit Borders** - Case-specific borders hold modules without permanent modifications

## Example Components

This proof of concept includes designs for:

- Power distribution panel
- Network switch module
- Raspberry Pi module (ATAK server)
- Cooling fan module
- Meshtastic node integration
- Ethernet and SMA antenna pass-throughs

Specific equipment choices are for demonstration. Users should customize components for their use case.

## Supported Cases

Borders are currently available for:
- Pelican 1400
- Strongway 13" frame

New borders can be designed for other cases while reusing all internal modules.

## Contributing

This is a proof of concept. All CAD files are provided in FreeCAD format for modification.

## License

See LICENSE file for details.

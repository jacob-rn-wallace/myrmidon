# Myrmidon

**Myrmidon** is an open source preservation, restoration, and reverse engineering project for the **iRobot PackBot 510** — a military-grade unmanned ground vehicle whose documentation, parts, and support infrastructure are not publicly available.

The PackBot 510 is no longer manufactured. Original iRobot support documentation, repair parts, and accessories are not publicly available, and the platform relies on military-spec consumables — including the BB-2590 battery — that have no civilian equivalent. Myrmidon exists to change that.

This README intentionally avoids implementation specifics. Hardware findings, firmware reverse engineering, and parts documentation are recorded in their respective directories.

---

## Project Vision

The goal of Myrmidon is to make the PackBot 510 **indefinitely serviceable** — not merely repairable with donor parts from other failing units, but supported by a complete, open library of documented internals, reproducible components, and understood protocols and interfaces.

This means:

- Full electrical documentation of the PackBot 510 chassis, drive system, and power interface
- A replica or civilian-compatible replacement for the BB-2590 military battery
- Reverse-engineered firmware and communication protocols
- Open, reproducible replacement parts fabricable with hobbyist tools

---

## Design Philosophy

Myrmidon is guided by the following principles:

- **Measure first** — no specification or behavior is assumed; everything is verified against the physical unit
- **Civilian-accessible** — solutions must not depend on military-spec hardware, consumables, or supply chains
- **Open by default** — all findings, measurements, and designs are published under open licenses so the community can build on them without restriction
- **Buildability** — replacement parts and processes should be executable by a motivated individual with hobbyist tools, not specialist manufacturing equipment

---

## Repository Structure

```
myrmidon/
├── CONTRIBUTING.md          # Contribution guidelines
├── LICENSE-DOCUMENTATION    # CC BY 4.0 (documentation)
├── LICENSE-FIRMWARE         # GPL-3.0 (firmware and software)
├── LICENSE-HARDWARE         # CERN-OHL-S-2.0 (hardware designs)
├── README.md                # This file
├── battery/                 # BB-2590 documentation, replica design, power alternatives
├── docs/                    # Physical descriptions, teardown notes, project documentation
├── hardware/                # Schematics, PCB documentation, BOM
├── software/                # Firmware, drivers, host tools
├── parts/                   # Replacement parts sourcing, 3D models, fabrication guides
└── references/              # Datasheets, photographs, preserved community findings
```

---

## Current Status

The project is in its earliest stage. One physical specimen is in hand:

- **PackBot 510 chassis** — bare chassis, no payloads, no accessories, no tracks (wheels only); primary subject

Work completed to date:

- Full disassembly and reassembly of the chassis
- Internal disassembly of one BB-2590 military battery to understand internal structure

Active priorities:

- Get the robot operational using accessible control electronics, bypassing original internals
- Document the BB-2590 battery interface and design a civilian power alternative
- Begin electrical documentation of the chassis and drive system

---

## Contributing

The project currently needs people with experience in:

- Embedded systems and motor control
- Power electronics and battery design
- Hardware and firmware reverse engineering

If you own a PackBot 510 and are willing to contribute photographs, measurements, or disassembly notes, that is equally valuable.

Please open an issue or discussion before proposing major architectural changes so that design intent can be preserved.

---

## Prior Art and Related Work

The only known public hands-on documentation of the PackBot 510 comes from @Alpha10six on Twitter, who has independently refurbished several PackBot models. His work provided the disassembly guidance that started this project. Reach out to him before duplicating effort or making assumptions about undocumented systems.

- [@Alpha10six on Twitter](https://twitter.com/Alpha10six) — hands-on refurbishment and disassembly documentation for multiple PackBot models

---

## License

Myrmidon uses a split license model:

- **Hardware designs** are licensed under the **CERN Open Hardware License Version 2 – Strongly Reciprocal (CERN-OHL-S-2.0)** (see `LICENSE-HARDWARE`)
- **Firmware and software** are licensed under the **GNU General Public License v3.0 (GPL-3.0)** (see `LICENSE-FIRMWARE`)
- **Documentation** is licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)** (see `LICENSE-DOCUMENTATION`)

Unless otherwise noted, files are licensed according to the category they fall under.

---

Myrmidon is not affiliated with or endorsed by iRobot. "iRobot" and "PackBot" are trademarks of iRobot Corporation.

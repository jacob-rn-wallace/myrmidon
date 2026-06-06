# Contributing to Myrmidon

Contributions of any kind are welcome — measurements, photographs, firmware,
software, hardware design, CAD work, documentation, and sourcing
research are all equally valuable at this stage of the project.

Please open an issue or discussion before proposing major architectural changes
so that design intent can be preserved.

---

## Code of Conduct

Myrmidon is a technical project and this is a technical space.
Contributions are evaluated on their merits. Discussion should remain focused
on the work.

The short version: be direct, be honest, and be respectful. Criticism of ideas
is welcome and expected. Personal attacks, harassment, and dismissiveness are
not.

If you have a concern about conduct, open a private discussion with the
maintainer.

---

## What the project needs right now

The most urgent contributions are physical characterization of the PackBot
510 itself. If you have a unit and are willing to examine it:

- Internal photography (high resolution, all angles and subassemblies)
- Electrical measurements (connector pinouts, supply voltages, signal identification)
- Dimensional measurements of key mechanical components

If you do not have a unit but have relevant skills, the areas of greatest need
are listed in the README.

---

## How to contribute

**For measurements, photographs, and physical documentation:**
Open a GitHub issue with your findings, or submit a pull request placing files
in the appropriate directory. Either approach is welcome. If submitting a pull
request, follow the file naming and directory conventions below.

**For firmware / software:**
Open a discussion before beginning significant work so that implementation
decisions can be agreed on in advance. Submit changes as a pull request against
the `main` branch.

**For hardware design (PCB, mechanical):**
Open a discussion before beginning significant work. Submit KiCad files and
FreeCAD or equivalent exports as a pull request. Native format files are
preferred over exports alone.

**For documentation:**
Submit a pull request directly. No prior discussion needed for documentation
fixes or additions.

---

## File naming and directory conventions

Files should be named descriptively and in lowercase with hyphens, not spaces
or underscores — for example `main-pcb-top.jpg` rather than
`Main PCB Top.jpg` or `main_pcb_top.jpg`.

Place files in the directory that matches their type:

```
battery/                 — BB-2590 documentation, replica design, power alternatives
docs/                    — teardown notes, project documentation
hardware/photos/         — high resolution PCB and component photography
hardware/schematics/     — traced schematics
hardware/bom/            — component identification and sourcing
hardware/datasheets/     — component datasheets and specifications
software/                — firmware, drivers, host tools
parts/sourcing/          — replacement parts sourcing research
parts/cad/               — CAD models and print-ready files
parts/drawings/          — dimensioned drawings and measurement records
references/              — datasheets, preserved community findings
```

---

## Measurements

When submitting physical measurements, include:

- The tool used (caliper model, multimeter model, etc.)
- The unit's condition and approximate age if known
- Any relevant variant information — hardware revision, regional variant, etc.
- Any relevant context — surface condition, modification history, etc.

Measurements submitted as markdown tables in a GitHub issue are perfectly
acceptable. They do not need to be formatted as CAD files to be useful.

---

## License

By contributing to Myrmidon you agree that your contributions will be
licensed under the same terms as the component they belong to:

- Hardware designs: CERN-OHL-S-2.0
- Firmware and software: GPL-3.0
- Documentation: CC BY 4.0

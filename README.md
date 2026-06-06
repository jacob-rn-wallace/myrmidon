# modus-operandi

A template repository for open source preservation, restoration, and reverse
engineering projects.

---

## How to use this template

1. Create a new repository from this template (or copy it manually).
2. Rename the root directory to your project name.
3. Replace every `[BRACKETED PLACEHOLDER]` throughout all files with
   project-specific content.
4. Delete or rename directories that do not apply to your project — the default
   structure is a starting point, not a requirement.
5. Delete this file and rename `README.template.md` to `README.md`.

---

## Repository structure

```
modus-operandi/
├── .github/
│   └── ISSUE_TEMPLATE/
│       └── contributing-finding.md   # Issue template for contributions
├── CONTRIBUTING.template.md          # Contribution guidelines (fill in)
├── LICENSE-DOCUMENTATION             # CC BY 4.0 (documentation)
├── LICENSE-FIRMWARE                  # GPL-3.0 (firmware and software)
├── LICENSE-HARDWARE                  # CERN-OHL-S-2.0 (hardware designs)
├── README.md                         # This file — delete after setup
├── README.template.md                # Project README — rename to README.md
├── docs/                             # Project documentation, teardown notes
├── hardware/                         # Schematics, PCB documentation, BOM
├── software/                         # Firmware, drivers, tools
├── parts/                            # Replacement parts, sourcing, CAD
└── references/                       # Datasheets, photographs, preserved
                                      # community findings
```

### Adapting the directory structure

The default directories cover the most common cases. Projects vary
significantly — rename, add, or remove directories as needed and update
`README.template.md` and `CONTRIBUTING.template.md` to match. Some examples from
existing projects:

- A robotics project may split `hardware/` into `electrical/` and
  `mechanical/`, and add a `firmware/` directory
- A software-heavy project may not need `hardware/` or `parts/` at all
- A vehicle project may add `diagnostics/` and `safety/`

Whatever structure you choose, keep `CONTRIBUTING.template.md` in sync so contributors
know where to put things.

---

## License model

This template uses the same split license model as all projects in this family:

- **Hardware designs** — CERN-OHL-S-2.0
- **Firmware and software** — GPL-3.0
- **Documentation** — CC BY 4.0

The license files in this repository are the full texts of each license. Do not
replace them — they are already correct. Update the license section of your
project README to reference them accurately.

---

## Related projects

- [Millennium](https://github.com/[USERNAME]/millennium) — Logitech MX1000
- [Michiyuki](https://github.com/[USERNAME]/michiyuki) — Tomy i-SOBOT

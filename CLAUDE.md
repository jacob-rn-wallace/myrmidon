# CLAUDE.md — modus-operandi

modus-operandi is a template repository for open source preservation,
restoration, and reverse engineering projects. It is not a product project
itself — it is the common foundation that product projects are derived from.

---

## How to work on this repository

Changes here are changes to the template, not to any derived project. Before
editing any file, ask: does this change reflect a convention that should apply
to all derived projects, or is it specific to one? If the latter, it belongs
in that project's repository, not here.

When updating the template, derived projects are not automatically updated —
changes are applied to new projects going forward and backported to existing
ones manually.

---

## Files and what they are

**`README.template.md`** — the canonical project README. This is the file
that gets renamed to `README.md` in each derived project. Every section,
heading, and placeholder is intentional. Do not reorder sections or rename
headings without a clear reason; consistency across projects is the goal.

**`CONTRIBUTING.template.md`** — contribution guidelines template. Section order:
code of conduct → current needs → per-type contribution workflow → file naming
and directory conventions → measurements guidance → license agreement.

**`.github/ISSUE_TEMPLATE/contributing-finding.md`** — issue template for
physical documentation contributions (measurements, photography, sourcing,
protocol capture).

**`LICENSE-DOCUMENTATION`**, **`LICENSE-FIRMWARE`**, **`LICENSE-HARDWARE`** —
full license texts. Do not edit these. CC BY 4.0, GPL-3.0, and CERN-OHL-S-2.0
respectively.

**`docs/`**, **`hardware/`**, **`software/`**, **`parts/`**, **`references/`**
— default directory structure. Each contains a `.gitkeep`. These are the
starting point; derived projects rename and extend as needed.

---

## Conventions

**File naming:** lowercase with hyphens. Example: `main-pcb-top.jpg`, not
`Main PCB Top.jpg` or `main_pcb_top.jpg`.

**Directory naming:** lowercase, single word where possible.

**Placeholders:** all template placeholders use `[BRACKETED UPPERCASE]` format.
When searching for unfilled placeholders in a derived project, grep for `\[`.

**License model:** CERN-OHL-S-2.0 for hardware, GPL-3.0 for firmware and
software, CC BY 4.0 for documentation. This is fixed across all projects in
the family — do not substitute.

**README tone:** direct and technical. The top-level README intentionally
avoids implementation specifics; those belong in their respective directories.

---

## Derived projects

| Project | Subject | Repository |
|---|---|---|
| Millennium | Logitech MX1000 | jacob-rn-wallace/millennium |
| Michiyuki | Tomy i-SOBOT | jacob-rn-wallace/michiyuki |

Update this table when a new project is started from the template.
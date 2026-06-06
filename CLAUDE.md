# CLAUDE.md — Myrmidon

Myrmidon is an open source preservation, restoration, and reverse engineering
project for the iRobot PackBot 510 unmanned ground vehicle. The goal is to
fully document the platform so that hobbyists can repair, modify, and build
new parts for existing units — and ultimately to make the robot operable
without dependence on original iRobot hardware or military-spec consumables.

---

## Project status

The project is in its earliest stage. The robot has been fully disassembled
and reassembled with outside guidance, so the physical structure is understood
at a hands-on level. No electrical, firmware, or protocol work has been done
yet.

**What exists:**
- One bare PackBot 510 chassis (no payloads, no accessories, no tracks —
  wheels only)
- Removable antennae
- One dissected BB-2590 military battery, disassembled to understand internal
  structure

**What does not exist yet:**
- Electrical diagrams or measurements
- Any firmware or software
- Protocol documentation
- Replacement or replica parts

---

## Goals

**Near-term:** Get the robot operational in any capacity. The most tractable
path is probably to reuse the chassis and drive motors with different — more
accessible — control electronics, bypassing the original internals entirely
for now.

**Medium-term:** Break the robot's dependence on the BB-2590 military battery.
This includes understanding the battery interface, designing replica BB-2590
units, and identifying or designing civilian power alternatives that are
compatible with the PackBot's power system.

**Long-term:** Complete reverse engineering of the original platform —
electrical, firmware, and protocols — so the robot can be operated and
understood on its own terms.

---

## Battery work

Battery documentation and replica design are part of this project, not a
separate one. The BB-2590 is the PackBot's primary power source, and making
the robot usable requires either replicating it or replacing it. Both
directions are in scope.

---

## Key external reference

A hobbyist (@Alpha10six on Twitter) has independently refurbished several
PackBot models and provided the disassembly guidance that got this project
started. His work is the only known public hands-on documentation of this
platform. Reach out to him before duplicating effort or making assumptions
about undocumented systems — he may have already solved problems this project
will encounter.

---

## Information environment

There is almost no publicly available technical information about the
PackBot 510. This is expected given its intended user base. Assume that
anything not documented in this repository is unknown until measured or
traced directly. Do not fill gaps with plausible-sounding inferences.

---

## ITAR and export control

**Open question — not yet resolved.**

The PackBot 510 is a former controlled military item. Reverse engineering a
unit you own is generally understood to be legal, but publishing detailed
technical findings — particularly around communications interfaces, protocols,
or cryptographic systems — may implicate ITAR or EAR depending on specifics.

Do not make legal determinations here. Flag any findings that touch comms,
crypto, or payload interfaces as potentially sensitive and treat them as
requiring separate review before publication.

---

## Repository structure

The default modus-operandi structure applies as a starting point. Expect it
to evolve significantly as the project develops. Battery-related work lives
under a `battery/` directory at the root level.

---

## Conventions

Inherited from modus-operandi. File names: lowercase with hyphens. Directory
names: lowercase, single word where possible. Placeholders: `[BRACKETED
UPPERCASE]`. License model: CERN-OHL-S-2.0 (hardware), GPL-3.0 (firmware and
software), CC BY 4.0 (documentation).

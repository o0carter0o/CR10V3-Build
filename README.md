# CR-10 V3 Under-Frame Electronics Conversion

This repository documents a CR-10 V3 conversion built around an MKS Robin Nano v3.1, independent dual Z, a Micro Swiss NG direct-drive extruder, CR Touch, and a four-piece printed under-frame electronics enclosure.

Current enclosure release: **v1.1**.

## Repository contents

- [`enclosure/STL/print_ready`](enclosure/STL/print_ready) — nine print-ready enclosure parts
- [`enclosure/STEP/assembled`](enclosure/STEP/assembled) — authoritative assembled STEP
- [`enclosure/STEP/parts_print_orientation`](enclosure/STEP/parts_print_orientation) — editable individual parts oriented for printing
- [`enclosure/STEP/parts_global`](enclosure/STEP/parts_global) — individual parts in installed coordinates
- [`enclosure/Accessories`](enclosure/Accessories) — opening blanks, Robin Nano spacers, and center-support adapter
- [`klipper`](klipper) — reference printer, macro, Mainsail, and Moonraker configuration snapshots
- [`docs/BUILD_GUIDE.md`](docs/BUILD_GUIDE.md) — printer and enclosure build overview
- [`docs/WIRING.md`](docs/WIRING.md) — board assignments and CR Touch wiring
- [`docs/ENCLOSURE_BOM.md`](docs/ENCLOSURE_BOM.md) — enclosure hardware list
- [`docs/ENCLOSURE_NOTES.md`](docs/ENCLOSURE_NOTES.md) — assembly and electrical notes

## Enclosure printing baseline

- 0.4 mm nozzle
- 0.20 mm layers
- At least 4 walls/perimeters
- At least 5 top and bottom layers
- Print the main parts in the supplied orientation
- The main parts are designed to print without supports

The assembled STEP is the authoritative v1.1 geometry. The STL files are the ready-to-print deliverables.

## Configuration warning

The files in `klipper/` are reference material for this specific machine. They are not a universal drop-in configuration. Verify the board revision, pin assignments, thermistor types, motor directions, travel limits, probe offsets, heater behavior, and emergency shutdown before moving any axis or heating anything.

At minimum, replace the MCU `serial:` path in `printer.cfg` with the path reported by your own controller.

## Safety

This conversion places AC mains wiring and a power supply in a printed enclosure. Use proper strain relief, insulated terminals, protective-earth bonding, fusing, wire sizes, separation, and continuity testing. Mains work should be performed only by someone qualified to do it.

## Attribution

This enclosure is a derivative of HeyRay2's [CR-10 V2 Control Box Eliminator - Standalone Conversion](https://www.thingiverse.com/thing:4347673). See [`ATTRIBUTION.md`](ATTRIBUTION.md).

## License

- STEP, STL, and documentation: [CC BY 4.0](LICENSE-CC-BY-4.0.txt)
- Klipper configuration and original macros: [GPL-3.0-or-later](LICENSE-GPL-3.0.txt)

See [`LICENSE.md`](LICENSE.md) for the file-by-file scope and third-party notices.

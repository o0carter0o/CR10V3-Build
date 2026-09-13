# CR-10 V3 Build Guide

This build converts a CR-10 V3 from the external OEM electronics box to an under-frame electronics enclosure.

## Major hardware

| Area | Part |
|---|---|
| Controller | MKS Robin Nano v3.1 |
| Screen | MKS TS35 v2.0 |
| Host | Raspberry Pi 3B/3B+ |
| PSU | Mean Well LRS-350-24 |
| Extruder | Micro Swiss NG direct drive |
| Probe | CR Touch |

## Enclosure

The enclosure is split into four printed shell quadrants plus four lids and a center support. The assembled STEP is the source of truth for the released V1.1 geometry:

`enclosure/STEP/assembled/CR10V3_Control_Box_V1.1_Assembled.step`

Print-ready STL files are in:

`enclosure/STL/print_ready/`

The case is designed around a 45 mm closed height so the top sits flush with the top of the lower frame extrusions while maintaining about 5 mm of ground clearance with 30 mm feet.

## Printing baseline

- 0.4 mm nozzle
- 0.20 mm layer height
- PLA, PETG, ASA, or similar material appropriate for your printer environment
- At least 4 walls/perimeters
- At least 5 top and bottom layers
- Print the parts in the supplied STL orientation
- Do not add supports for the built-in zip-tie anchors; the anchor roof geometry was designed around short spans and angled faces.

Inspect screw pilots before assembly. The design uses direct-thread printed holes, not heat-set inserts.

## Assembly notes

- Mount the PSU directly through the enclosure ceiling.
- Use short PSU screws and verify they cannot penetrate too far into the power supply.
- Use M4 hardware and T-nuts for the frame mounts and center support clamp.
- Use M3 hardware for lids, board mounts, fans, and printed accessories unless noted otherwise.
- Use M2.5 hardware for the Raspberry Pi.
- Keep AC mains wiring physically separated from low-voltage and signal wiring.
- Check continuity, strain relief, earth bonding, and insulation before applying mains power.

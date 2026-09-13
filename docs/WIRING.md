# Wiring Notes

These notes document the intended CR-10 V3 electronics conversion. Verify against your own board silkscreen and pinout before powering anything.

## Controller

- Board: MKS Robin Nano v3.1
- Drivers: TMC2209 UART on X, Y, Z, E0, and E1
- Independent Z: second Z motor connected to E1
- FAN0: hot-end heatsink fan
- FAN1: layer cooling fan
- HE1 / spare heater output: case-fan testing/control target

## CR Touch

The OEM harness uses a 3-pin probe connector plus a separate D11 signal.

| CR Touch / harness side | Robin Nano v3.1 target |
|---|---|
| 3-pin probe connector | Z- header: PC8, GND, 5V |
| D11 signal | PA8 on BLTouch/sensor header |

The PA8 pin is the square pin on the referenced board diagram used during the build.

## Endstops and filament sensor

- X and Y endstops use the normal endstop inputs.
- The OEM two-pin endstop plug may need to be repinned into a three-pin housing.
- Filament sensor is assigned to Z+ in the working build notes.

## Power

- Main PSU: 24 VDC output from Mean Well LRS-350-24
- Raspberry Pi power preference: dedicated 24 V to 5 V buck converter
- Case fans: planned through a 24 V to 12 V buck when using 12 V fans

## Safety

This enclosure contains mains voltage. Use insulated terminals, appropriate wire gauge, proper strain relief, protective earth bonding, fusing, and separation between mains and low-voltage wiring.


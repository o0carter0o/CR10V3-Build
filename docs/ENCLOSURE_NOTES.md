# V1.1 Notes

## Changes from V1.0

- Left Rear: rear keystone replaced by a second Ø17 mm grommet opening.
- Robin Nano: all eight optional mounting bosses now use the short geometry; use four 5 mm spacers in either board position.
- Right Rear: keystone moved slightly toward machine center and given an internal snap-fit cage with a 45° printable underside.
- Right Rear: added a Ø4.5 mm frame-bond access hole and protective-earth symbol.

Part filenames use installed machine position, viewed from the front/operator side of the printer. Earlier internal CAD/package naming had left and right reversed; this repo uses the corrected installed-position names.

## Assembly notes

- Insert the Left Rear keystone from inside the enclosure toward the exterior.
- The built-in zip-tie anchors are intended to print without support. Avoid support material inside the tie channels; it adds cleanup risk without helping the final part.
- Use the supplied print orientation for the shell quadrants and lids.
- Direct-thread the printed pilots carefully. Start screws square to the hole and avoid over-tightening.
- The center support clamps the inner quadrant corners to the central 20×40 extrusion from inside the enclosure.
- Twist the internal switched Line and Neutral run from the inlet/switch area to the PSU.
- Twist or closely couple the internal `+24 V / 0 V` pair from the PSU to the Robin Nano.
- If the keystone carries normal data, an inlet-mounted EMI filter or grounded L-shaped steel divider may be added if desired.
- If Cat6 carries steppers/endstops, keep each motor coil on one twisted pair and place endstop signal/ground on their own pair.

Frame bonding is an optional retrofit in this design and is strongly encouraged when modifying the mains enclosure. The designer's personal solution is a suitable self-tapping screw through the marked hole into the extrusion V-channel with a ring terminal and toothed washer. This permanently marks/cuts the extrusion and is not readily reversible.

Alternatives include enlarging the access for a conductive T-nut and ring terminal, drilling and tapping the frame, routing the bonding wire to another suitable frame location, or bonding the grounded PSU chassis to the printer frame. Any method must make reliable metal-to-metal contact; verify continuity after assembly. Mains work should be performed only by someone qualified to do it.

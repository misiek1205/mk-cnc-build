# Commissioning and safety minimum

This build pack covers the mechanical machine. Do not run the machine until
the following minimum checks have been completed.

## Required before a first powered move

- Fit an accessible emergency stop that removes power from the spindle and
  motion system. A software stop alone is not an emergency stop.
- Fit normally-closed limit switches at both ends of X and Z, and one at each
  Y home position. The two Y motors must be homed independently so the gantry
  can square itself on every homing cycle.
- Configure and test the correct travel limits, homing direction and soft
  limits with the spindle disconnected.
- Bond exposed conductive machine parts and the spindle body to protective
  earth. Provide strain relief for the spindle and drag-chain cables.
- Jog each axis through its full usable travel at low speed. Check that the
  screw, coupler, nut, carriage and cable path cannot contact the frame,
  table or workpiece at either limit.

## Mechanical setup

1. With the machine unpowered, loosen one rail of each parallel rail pair,
   move the carriage through its travel, then tighten progressively. It must
   move freely without a cyclic tight spot.
2. Home Y and measure the gantry-to-frame distance on both sides. Repeat after
   several power cycles; a changing measurement means the two Y drives are not
   being squared reliably.
3. Set the table height and workholding so the installed tool can reach the
   spoilboard without the Z plate, collet nut, dust shoe or motor tower reaching
   a hard stop.
4. Start with wood or plastic and conservative cutting parameters. The printed
   structure and 2020 frame are not intended for aggressive aluminium machining.

## Release check for a published build

- Record the exact cut lengths for every 2020 profile and the rail/screw
  lengths used by the reference machine.
- State the tested controller, the independent-Y homing arrangement and the
  endstop locations.
- Slice every STL with the release slicer profile and resolve any mesh-repair
  warning before publishing the final archive.

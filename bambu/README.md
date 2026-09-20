
> **WIP:** plate layout may still change as the machine design evolves.

﻿# Bambu Studio print projects

Ready-to-open multi-plate `.3mf` files for the MK CNC printed parts.

| File | Printer | Bed | Plates |
|------|---------|-----|--------|
| `MK_CNC_P1S.3mf` | Bambu Lab **P1S** (0.4 nozzle) | 256 mm | 6 |
| `MK_CNC_A1_mini.3mf` | Bambu Lab **A1 mini** (0.4 nozzle) | 180 mm | 13 |

## Profile (both)

- Filament: **Bambu PLA Basic** (change to PETG/ASA in Studio if you want)
- Layer height: **0.2 mm**
- Walls: **6**
- Top / bottom: **5**
- Infill: **Adaptive Cubic** ~40% (50% on load-bearing parts: Z plate, X nut, spindle/Makita holders; 30% on laser/pen)
- Supports: **off**
- Orientations match the STL files (do not rotate)

Includes required parts **and** optional Makita / laser / pen holders.

## How to use

1. Open the `.3mf` in **Bambu Studio**.
2. Confirm printer (P1S or A1 mini) and filament.
3. Slice each plate and print (or send the plate you need).
4. First open may ask Studio to refresh thumbnails — that is normal.

If anything looks odd on the bed, use **Auto Arrange** on that plate, then re-slice.

## Note

These projects are generated for MakerWorld / click-to-print. Individual STL files remain in `../stl/` if you prefer to place parts yourself.

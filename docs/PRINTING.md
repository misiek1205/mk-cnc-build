# Printing guide

All files in `stl/` are already oriented for printing. **Do not rotate** them in the slicer.  
**No supports** are required when printed as oriented.

`L` / `R` = left / right from the operator (front = spindle).

Preview sheet: [img/parts_print_sheet.png](img/parts_print_sheet.png)

## Shared slicer settings

| Setting | Value |
|---------|--------|
| Material | **PLA**, **PETG**, or **ASA** — all fine for this machine when printed as below. Reference build used **Bambu Basic PLA**. PETG/ASA if you want more heat resistance or less creep. |
| Nozzle | 0.4 mm |
| Layer height | 0.2 mm |
| Perimeters | **6** (~2.4 mm shell) |
| Top / bottom | **5** layers |
| Infill | **Adaptive Cubic** (or similar) |
| Elephant foot / negative horiz. expansion | Keep bearing seats dimensional |
| Supports | **Off** |

Do **not** print at 100% infill. With 6 perimeters, thin ribs are already nearly solid.

## Part list

| STL | Qty | On bed | Infill | Notes |
|-----|-----|--------|--------|-------|
| `leg_L.stl` / `leg_R.stl` | 1+1 | Outer wall | 40% | Beam pocket opens sideways |
| `leg_cap_L.stl` / `leg_cap_R.stl` | 1+1 | Flat | 40% | |
| `y_motor_bracket_L.stl` / `y_motor_bracket_R.stl` | 1+1 | Motor plate | 40% | Ribs up |
| `y_bearing_block_L.stl` / `y_bearing_block_R.stl` | 1+1 | Tab with M5 | 40% | 608 bore horizontal |
| `side_tie_plate.stl` | 12 | Flat | 40% | |
| `x_motor_bracket.stl` | 1 | Motor plate | 40% | Ribs + wedge up |
| `x_bearing_block.stl` | 1 | Bearing plate | 40% | 608 pocket opens up |
| `x_carriage.stl` | 1 | Side (+X face) | 40% | Height ~105 mm; C-channel sideways |
| `x_nut_block.stl` | 1 | Face toward carriage | 50% | |
| `z_plate.stl` | 1 | Back face | 50% | |
| `z_motor_tower.stl` | 1 | Motor plate | 40% | Collars up; **side T-slots free** |
| `spindle_holder_52.stl` | 1 | Base back | 50% | Default tool |
| `spindle_clamp_cap.stl` | 2 | Flat | 50% | |
| `makita_holder_65.stl` | 0–1 | Optional | 50% | |
| `makita_clamp_cap.stl` | 0–2 | Optional | 50% | |
| `laser_adapter.stl` | 0–1 | Optional | 30% | Nut channels on bed |
| `pen_holder.stl` | 0–1 | Optional | 30% | |
| `dust_shoe_52.stl` | 1 | Flat on bed | 40% | Optional; ø52; clamp slot + 2× M4; upward ø35 hose |

Individual previews: `docs/img/part_<name>.png`.

## Bambu Studio projects

- `bambu/MK_CNC_P1S.3mf` — **18 named plates**, max 2 parts each (side ties share plate 03). Plates **01–13** = required build order; **14–18 OPTIONAL** = Makita / laser / pen / dust shoe.
- `bambu/MK_CNC_A1_mini.3mf` — **21 named plates** (smaller bed splits some pairs). Same stage names; dust shoe is a single optional plate.
- Settings: 0.2 mm, 6 walls, gyroid-style sparse, PLA Basic, supports off.
- Keep the stage names; skip plates whose title starts with **OPTIONAL** if you do not need those tools.

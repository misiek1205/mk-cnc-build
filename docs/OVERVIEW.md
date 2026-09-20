# Machine overview

## Philosophy

MK CNC is a **small moving-gantry mill** whose printed parts adapt scavenged aluminium extrusion, linear rails, leadscrews and steppers into one coherent machine. Dimensions in the BOM match a typical leftover pile from old 3D printers; shorter screws or rails simply reduce travel — the printed parts still fit.

## Layout

- **Base:** plywood plate with 2020 runners and side stacks.
- **Y axis:** gantry (40×40 mm effective beam from 2×2 2020) on MGN12 rails; two T8 screws driven by NEMA17 motors at the rear.
- **X axis:** carriage on dual MGN12 on the beam; one T8 screw behind the beam (motor behind left leg, 608 bearing behind right leg).
- **Z axis:** twin 2020 columns on the carriage front; dual MGN12; T8 in the middle; motor on a printed tower; tool on a universal Z plate.

| Axis | Nominal travel |
|------|----------------|
| X | ~299 mm |
| Y | ~271 mm |
| Z | ~100 mm |

Largest circular pocket with a ø6 mm endmill in one fixture (reference): about **ø277 mm** (Y-limited).

## Coordinates

- **+Y** = machine front (operator / spindle side)
- **+X** = operator's **left**
- **+Z** = up

If you want GRBL “X+ = right from the operator”, invert the X motor in firmware.

## Naming

`*_L` / `*_R` = **Left / Right from the operator** standing in front of the spindle.  
`L` parts sit on the **+X** side of the model.

## Tool interface

Z plate has a 4× M4 pattern. Swap:

- `spindle_holder_52` — ø52 spindle (default)
- `makita_holder_65` + caps — Makita RT0700 / DRT50 style
- `laser_adapter` — T-slot plate for laser modules
- `pen_holder` — pen / marker clamp
- `dust_shoe_52` - one-piece vacuum dust shoe for the ø52 spindle (clamp slot + 2× M4, upward ø35 hose)

---

## Assembly renders

![Front-right isometric](img/assembly_iso_front_right.png)

![Front-left isometric](img/assembly_iso_front_left.png)

![Rear isometric](img/assembly_iso_rear.png)

![Mechanics without table](img/assembly_mechanics_no_table.png)

![Carriage / Z close-up](img/closeup_carriage_iso_front.png)

![Left leg close-up](img/closeup_leg_L_iso.png)

![Z axis close-up](img/closeup_z_axis_iso_front.png)

![Dust shoe on spindle (front iso)](img/closeup_dust_shoe_iso_front.png)

![Dust shoe from below](img/closeup_dust_shoe_iso_low.png)

![Dust shoe side](img/closeup_dust_shoe_side_L.png)

![Dust shoe section — continuous vacuum tunnel](img/closeup_dust_shoe_tunnel_section.png)

![Print orientation sheet](img/parts_print_sheet.png)

---

## Printed parts (previews)

### Structure

![leg_L](img/part_leg_L.png)

![leg_R](img/part_leg_R.png)

![leg_cap_L](img/part_leg_cap_L.png)

![leg_cap_R](img/part_leg_cap_R.png)

![side_tie_plate](img/part_side_tie_plate.png)

### Y axis

![y_motor_bracket_L](img/part_y_motor_bracket_L.png)

![y_motor_bracket_R](img/part_y_motor_bracket_R.png)

![y_bearing_block_L](img/part_y_bearing_block_L.png)

![y_bearing_block_R](img/part_y_bearing_block_R.png)

### X axis

![x_motor_bracket](img/part_x_motor_bracket.png)

![x_bearing_block](img/part_x_bearing_block.png)

![x_carriage](img/part_x_carriage.png)

![x_nut_block](img/part_x_nut_block.png)

### Z axis / tools

![z_plate](img/part_z_plate.png)

![z_motor_tower](img/part_z_motor_tower.png)

![spindle_holder_52](img/part_spindle_holder_52.png)

![spindle_clamp_cap](img/part_spindle_clamp_cap.png)

![makita_holder_65](img/part_makita_holder_65.png)

![makita_clamp_cap](img/part_makita_clamp_cap.png)

![laser_adapter](img/part_laser_adapter.png)

![pen_holder](img/part_pen_holder.png)

![dust_shoe_52](img/part_dust_shoe_52.png)


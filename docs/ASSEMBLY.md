# Assembly guide

Coordinates match [OVERVIEW.md](OVERVIEW.md). Measure profile hole positions **from the end of each extrusion**.

Read the **trap list** at the end before you torque everything down.

## 1. Print

See [PRINTING.md](PRINTING.md). Dry-fit: 608 bearings push in by hand; `x_nut_block` width matches the carriage; `z_motor_tower` collars slide onto column tops.

## 2. Cut and tap aluminium

- Cut the reference-machine 2020 profiles to length:

  | Element | Qty | Cut length |
  |---------|----:|-----------:|
  | Bridge beam (2×2 2020) | 4 | 500 mm |
  | Runners / crossbars | 4 | 420 mm |
  | Sides | 4 | 380 mm |
  | Z columns | 2 | 240 mm |

  The matching reference rails are X 2×400 mm, Y 2×380 mm and Z 2×220 mm;
  the screws are X 400 mm, Y 2×350 mm and Z 200 mm. See
  [BOM.md](BOM.md#reference-geometry) for the complete reference geometry.
- Tap centre holes M5 where screws go into the profile core (leg end walls, Z tower tops).
- Drill ø5.5 through the beam stack for the 12 clamp bolts (slide-in T-nuts).

## 3. Base and sides

1. Build left/right side stacks (extrusion + `side_tie_plate` ×12).
2. Mount Y rails; leave one rail slightly loose until the gantry walks true, then tighten hole-by-hole.
3. Fit `y_motor_bracket_L` / `_R` at the rear — T-nuts in the inner slots **before** you lose access.
4. Fit `y_bearing_block_L` / `_R` at the front.

## 4. Legs and gantry beam

1. Assemble the 2×2 beam: insert **12× M5 T-nuts** into the inner slots **before** you close the stack.
2. Seat `leg_L` / `leg_R` on the Y carriages; clamp the beam into the leg pockets.
3. Add `leg_cap_L` / `_R`: slide captive M3 nuts into the slots first, then cap screws.
4. Mount Y anti-backlash nuts on the leg arms: **ø22 flange flat on the print**, spring outside.

## 5. X drive and carriage

1. Mount `x_motor_bracket` (behind left leg) and `x_bearing_block` (behind right leg) on the rear face of the beam.
2. Install X screw, coupler, 608 bearing.
3. Slide `x_carriage` onto the X rails; square the rails (one tight, one loose, walk the carriage).
4. Fit `x_nut_block` to the carriage rear; nut flange flat against the block, spring outside.
5. Insert column T-nuts into the carriage front pockets **before** bolting Z columns.

## 6. Z axis

1. Bolt Z columns to the carriage; mount Z rails and carriages.
2. Fit `z_plate`; insert M4 hex nuts into the rear pockets.
3. Mount Z anti-backlash nut on top of the plate (spring in free air).
4. Slide `z_motor_tower` onto the column tops: **tenons only in front/rear slots**; install side M5 T-nuts **before** dropping the tower.
5. Motor M3 from **below** the tower plate; rear pair via the access ovals between the columns.
6. Attach `spindle_holder_52` (or another tool) to the Z interface.

## 7. Table and electrics

- Fit plywood base and MDF table so Z can reach the surface.
- Wire steppers, endstops and spindle PSU to your controller. Firmware is out of scope of this pack.
- Before powering the spindle, complete [COMMISSIONING.md](COMMISSIONING.md). In particular, the two Y motors require independent homing against separate Y switches so the gantry is squared at every homing cycle.

## Assembly traps

1. **T-nuts before you block access** — beam stack, carriage column pockets, Z tower side slots, laser adapter channels.
2. **Rail parallelization** — never torque both rails fully before walking a carriage/plate.
3. **Do not rotate STLs** — legs and carriage print on their side for a reason.
4. **608 bearings** — finger press; lead-ins are in the STLs; no hammer.
5. **Anti-backlash nuts** — flat ø22 on plastic, spring outside; only the screw goes through the hole.
6. **L/R mirrors** — check pocket / nut-arm handedness before printing a second side.
7. **Z motor screws** from below; start threads before fully seating the coupler if the oval is tight.

## Closest images

- Legs: `img/closeup_leg_L_iso.png`
- Carriage / Z: `img/closeup_carriage_iso_front.png`
- Full machine: `img/assembly_iso_front_right.png`

## Optional: dust shoe (ø52 spindle)

One-piece stadium/capsule shoe with a **clamp slot** on the spindle and a single **upward** ~ø35 vacuum port:

1. Print `dust_shoe_52` (flat on bed). In the Bambu projects it is plate **18 OPTIONAL Dust shoe** (`dust_shoe_52`).
2. Slip the shoe onto the spindle body **below** the lower spindle clamp (remove the endmill / ER nut if needed).
3. Close the clamp slot with **2× M4** through the ears (hose-clamp style).
4. Push a ~ø35 vacuum hose onto the **upward** stub. For ø32 hoses, use a short reducer sleeve.
5. Air path is continuous: bit chamber → plenum → hose (no separate elbow).

## Optional: endstop mounts

Print `endstop_mount_2020` ×4 (T-slot key + M5 into a T-nut; endstop on 2× M3 through slots) and optional `endstop_flag` ×0–4.

Placement (no holes in aluminium):

1. **Y-L / Y-R** (dual-Y squaring): outer face of each upper side 380 near the rear (Y motors).
2. **X home**: rear face of the bridge near the X motor.
3. **Z home (up)**: front face of a Z column just under the motor tower.

With only three switches: fit **Y-L + Y-R + Z** first.

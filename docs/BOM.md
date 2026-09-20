# Bill of materials — shopping list

Simple buy list for the **reference** machine (X travel ~299 mm, Y ~271 mm, Z ~100 mm).

**Prices** are approximate **AliExpress / China marketplace** ballparks in **EUR**, mid-2026, shipping excluded. Local EU shops are often 1.5–3× higher. Treat costs as a guide, not a quote.

## Reference geometry

These are the cut lengths for the documented reference machine. Measure cut
length from end to end; they are not the nominal work travel.

| Component | Qty | Length | Notes |
|-----------|----:|-------:|-------|
| 2020 bridge beam | 4 | 500 mm | 2×2 2020 beam |
| 2020 runners / crossbars | 4 | 420 mm | Base members |
| 2020 sides | 4 | 380 mm | Side stacks |
| 2020 Z columns | 2 | 240 mm | Carriage to Z tower |
| MGN12 X rail | 2 | 400 mm | With MGN12H carriages |
| MGN12 Y rail | 2 | 380 mm | |
| MGN12 Z rail | 2 | 220 mm | Often cut from 350 mm rails |
| T8 X screw | 1 | 400 mm | 8 mm lead typical |
| T8 Y screw | 2 | 350 mm | 8 mm lead typical |
| T8 Z screw | 1 | 200 mm | Prefer 2 mm lead for self-locking |

Shorter rails or screws can be used if they fit the printed interfaces, but
they reduce the stated travel and must be checked for end-of-travel collisions.

## 1. Buy this (mechanics)

| # | What to buy | Qty | ~EUR each | ~EUR total | Notes |
|---|-------------|-----|-----------|------------|-------|
| 1 | MGN12 rail **400 mm with MGN12H carriage** | 2 | 14 | 28 | X axis |
| 2 | MGN12H carriage (loose) | 3 | 5 | 15 | Need **12** carriages total (4Y+4X+4Z); buy the rest if your scrap pile is short |
| 3 | T8 leadscrew **400 mm** + anti-backlash nut | 1 | 8 | 8 | X; 8 mm lead typical |
| 4 | T8 leadscrew **350 mm** + anti-backlash nut | 2 | 7 | 14 | Y |
| 5 | T8×**2 mm** leadscrew ~**200 mm** + anti-backlash nut | 1 | 8 | 8 | Z; 2 mm lead preferred (self-locking) |
| 6 | 608-2RS ball bearing | 3 | 1 | 3 | Only if you do not already have them |
| 7 | Flexible coupler 5×8 mm | 4 | 2 | 8 | Only if missing from old printers |
| 8 | M5 T-nuts for 2020 | ~120 | — | 8 | Bulk bag |
| 9 | M3 T-nuts for 2020 | ~100 | — | 6 | Bulk bag |
| 10 | Assorted screws (M3 / M4 / M5) + hex nuts | 1 kit | — | 15 | See fastener table below if you buy individually |
| | **Subtotal mechanics (typical)** | | | **~€110** | Assumes you still need most carriages/couplers |

If you already have rails, screws, steppers and T-nuts from old printers, the **extra buy** is often only items 1–5 → roughly **~€60–80**.

## 2. Buy this (tool + sheet goods)

| # | What to buy | Qty | ~EUR | Notes |
|---|-------------|-----|------|-------|
| 11 | DC spindle ~500 W, body **ø52**, ER11 + matching PSU | 1 | 50–80 | Skip if you reuse another tool |
| 12 | Plywood 18 mm, ~480 × 500 mm | 1 | 15–25 | Base plate (local timber yard) |
| 13 | MDF 18 mm, ~404 × 287 mm | 1 | 8–15 | Sacrificial table |
| 14 | M6 wood inserts (table grid) | ~12 | 3 | Optional fixture grid |

## 3. Usually scavenged (check your shelf first)

Do **not** buy these if you already have them from old 3D printers:

| Item | Qty needed | Typical source |
|------|------------|----------------|
| 2020 aluminium extrusion (cut to length) | sides, 2×2 beam, Z columns, crossbars | printer frames / leftover stock |
| MGN12 rails (Y / Z) | 2×380 mm / 2×220 mm | old printers; see reference geometry above |
| NEMA17 steppers | 4 | old printers |
| 5×8 couplers, 608 bearings | 4 + 3 | old printers |
| M3 / M5 T-nuts and screws | see below | leftover bags |

## 4. Anti-backlash nuts (important)

Buy the common brass spring T8 nuts:

- mounting flange **ø22**
- 4× M3 on ~16 mm PCD
- spring + small retainer on the outside

**Mount:** flange flat on the printed part, spring stack **outside** the plastic. The hole only needs to clear the leadscrew.

## 5. Fastener counts (if buying loose)

Approximate, buy **+10%** spare:

| Use | Screw | Qty |
|-----|-------|-----|
| Y / X / Z rails | M3×8 | ~80 |
| Carriages → legs / X carriage | M3×16 | 32 |
| Carriages → Z plate | M3×20 | 16 |
| Y anti-backlash nuts | M3×25 | 8 |
| X / Z anti-backlash nuts | M3×12 | 8 |
| Y motors | M3×16 | 8 |
| X / Z motors | M3×10 / M3×16 | 4 + 4 |
| Legs ↔ beam | M5×16 / M5×30 | 8 + 8 |
| Leg caps | M5×16 + M3×16 | 4 + 8 |
| Tool → Z plate | M4×25 (laser: M4×30) | 4 |
| Beam clamp (2×2) | M5×30 | 12 |
| Y motor / bearing / side ties / brackets | M5×12 / M5×16 / M5×20 | ~70 |
| X nut block → carriage | M4×30 | 4 |
| Z columns / tower / spindle clamps | M5×16 / M5×40 / M4×40 | 6 + 2 + 4 |

## 6. Optional tools (print parts already in `stl/`)

| Tool | Extra buy | STL |
|------|-----------|-----|
| Makita RT0700 / DRT50 style (ø65) | router if you do not own one | `makita_holder_65` + caps |
| Laser module | module + PSU | `laser_adapter` |
| Pen / marker | — | `pen_holder` |
| Dust shoe for ø52 spindle | Hose ~ø35 ID, upward port; clamp slot + 2× M4 | `dust_shoe_52` (qty 1) |

## Ballpark totals

| Scenario | ~EUR |
|----------|------|
| You have extrusion, steppers, many T-nuts; buy rails/screws/carriages only | **60–80** |
| Full mechanics buy (little scrap) | **~110** |
| + spindle + sheet goods | **+70–120** |
| **Complete kit from almost nothing** | **~180–230** |

Controller, endstops, wire and PSU for steppers are **not** listed — pick your own (GRBL, FluidNC, etc.).

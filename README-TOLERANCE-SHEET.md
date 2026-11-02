# Solwright™ Precision Architectural Lattice Sampler (3-Panel .svg & AutoCAD Release 2010 .dxf Pack)

**Studio:** Solwright™ Precision Vector Studio (`snowfieldhq+solwright@atomicmail.io`)  
**Storefront:** https://solwright.itch.io/  
**Custom 6-Piece Campaign Commission ($250.00 flat, 72-hour turnaround):** https://snowfieldhq.neocities.org/solwright-vector-campaigns.html  
**License:** Free commercial and personal evaluation sampler (`$0.00`). Zero generative image models used (`100.0%` symbolic coordinate construction via Python `sympy` + `shapely` + `ezdxf`).

---

## Panel Specifications and Verified Geometric Audit

| Panel ID | Architectural Motif | Mathematical Construction Law (`256 x 256` Master Grid) | Closed Apertures | SVG Audit Score & Anchors | AutoCAD Release 2010 `.dxf` Entities | Min Bridge (`256` Grid / `24 in` Panel) |
| :--- | :--- | :--- | :---: | :---: | :--- | :---: |
| **`SW-P01`** | Seed-of-Life Vesica Rosette Lattice Panel | Outer circle R=112; central oculus r=20; 6 radial Vesica Piscis petals (R=38, sep=46 at R=62); 6 spandrel oculi (r=12 at R=78) | `13` | **`100/100`** (`42` anchors, `0` warnings) | `R2010` (`8` native `CIRCLE`s, `6` closed `LWPOLYLINE`s, `12` true arc bulges, `0` audit errors) | `11.75` units / **`1.259` in** |
| **`SW-P02`** | Octagonal Rub el Hizb Mashrabiya Screen Panel | Outer regular octagon (apothem 108, edges 0/45/90/135 deg); central Rub el Hizb 8-star (a=26); 4 cardinal 45-deg diamond lights; 4 diagonal oculi (r=14 at R=70) | `9` | **`100/100`** (`58` anchors, `0` warnings) | `R2010` (`4` native `CIRCLE`s, `6` closed `LWPOLYLINE`s, `0` true arc bulges, `0` audit errors) | `11.23` units / **`1.203` in** |
| **`SW-P03`** | Dodecagonal Gothic Lancet Tracery Panel | Outer regular 12-gon (R=114, rot 15 deg); central regular hexagon (r=18); 3 pointed lancet vesicae (R=42, sep=50 at R=62); 3 circular rose oculi (r=15 at R=68) | `7` | **`100/100`** (`38` anchors, `0` warnings) | `R2010` (`3` native `CIRCLE`s, `5` closed `LWPOLYLINE`s, `6` true arc bulges, `0` audit errors) | `12.66` units / **`1.356` in** |

## CAD / CAM / Plotter Import Notes

1. **Zero open contours or stacked duplicate lines:** Every `.svg` file uses a single boolean-validated compound `<path fill-rule="evenodd">` with analytical circular `A` arcs and `L` segments. Every `-R2010.dxf` file separates `OUTER_PROFILE` (Layer 1) from `INNER_APERTURE` cutouts (Layer 2) using native `CIRCLE` entities and closed `LWPOLYLINE` bulge arcs (`bulge = tan(sweep / 4)`).
2. **Scaling for Computer Numerical Control routers, laser cutters, and waterjets:** The master coordinate grid spans `224` to `228` units inside a `256 x 256` viewBox. Scaling `1` unit to `2.5` millimeters yields a `560 mm x 560 mm` (`~22 in`) decorative screen with minimum structural bridge widths between `19.2 mm` (`0.756 in`) and `26.2 mm` (`1.031 in`), well above the `3.81 mm` (`0.150 in`) cabinetry plywood and cellular polyvinyl chloride router floor.
3. **Need a custom 6-piece mathematical vector campaign tailored to your exact bit diameter, laser kerf, or brand proportions?** Order the fixed-scope **$250.00** Solwright™ Campaign Pack (`6` bespoke `.svg` + Release 2010 `.dxf` + dimensioned `.pdf` pieces in `72` hours) at: https://snowfieldhq.neocities.org/solwright-vector-campaigns.html

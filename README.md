# Solwright™ Architectural Lattice Precision Sampler (`SW-P01`, `SW-P02`, `SW-P03`)

Three non-generative Constructive Solid Geometry (`CSG`) architectural lattice panels in Scalable Vector Graphics (`.svg`) and AutoCAD Release 2010 Drawing Exchange Format (`.dxf`), constructed deterministically with Python (`sympy`, `shapely`, and `ezdxf`).

- **Custom 6-Piece Mathematical Vector Campaign (`$250.00` flat, 72-hour turnaround):** https://snowfieldhq.neocities.org/solwright-vector-campaigns.html (`1 campaign * $250.00 = $250.00` gross; `$250.00 - ($250.00 * 0.033 + $0.30) = $241.45` net after standard card processing)
- **GitHub Pages Mirror:** https://snowfieldhq.github.io/solwright-vector-campaigns.html
- **`$0.00` Downloadable Pack on itch.io:** https://solwright.itch.io/architectural-lattice-sampler
- **Direct Studio Intake:** `snowfieldhq+solwright@atomicmail.io`

---

## Verified Geometric Audit & Bridge-Width Table

| Panel ID | Architectural Motif | Symmetry | Mathematical Construction Law (`256 x 256` Grid) | Closed Apertures | SVG Audit Score & Anchors | AutoCAD Release 2010 `.dxf` Entities | Min Bridge (`256` Grid) | Min Bridge at `24 in` Panel (`bridge / 224 * 24 in`) |
| :--- | :--- | :---: | :--- | :---: | :---: | :--- | :---: | :---: |
| **`SW-P01`** | Seed-of-Life Vesica Rosette Lattice Panel | `D6` (`6`-fold) | Outer circle `R=112`; central oculus `r=20`; `6` radial Vesica Piscis petals (`R=38`, `sep=46` at `R=62`); `6` spandrel oculi (`r=12` at `R=78`) | `13` | **`100 / 100`** (`42` anchors, `1,395` B) | `AC1024` (`8` `CIRCLE` + `6` closed `LWPOLYLINE`, `12` arc bulges, `0` errors) | `11.75 u` | **`1.259 in`** (`31.98 mm`) |
| **`SW-P02`** | Octagonal Rub el Hizb Mashrabiya Screen Panel | `D8` (`8`-fold) | Outer regular octagon (apothem `108`, edges `0/45/90/135` deg); central Rub el Hizb `8`-star (`a=26`); `4` cardinal `45`-deg diamond lights; `4` diagonal oculi (`r=14` at `R=70`) | `9` | **`100 / 100`** (`58` anchors, `1,184` B) | `AC1024` (`4` `CIRCLE` + `6` closed `LWPOLYLINE`, `0` arc bulges, `0` errors) | `11.23 u` | **`1.203 in`** (`30.56 mm`) |
| **`SW-P03`** | Dodecagonal Gothic Lancet Tracery Panel | `D12` (`12`-fold) | Outer regular `12`-gon (`R=114`, rot `15` deg); central regular hexagon (`r=18`); `3` pointed lancet vesicae (`R=42`, `sep=50` at `R=62`); `3` circular rose oculi (`r=15` at `R=68`) | `7` | **`100 / 100`** (`38` anchors, `996` B) | `AC1024` (`3` `CIRCLE` + `5` closed `LWPOLYLINE`, `6` arc bulges, `0` errors) | `12.66 u` | **`1.356 in`** (`34.45 mm`) |

---

## Panel Previews

| `SW-P01` Seed-of-Life Vesica Rosette | `SW-P02` Octagonal Mashrabiya Screen | `SW-P03` Dodecagonal Gothic Lancet |
| :---: | :---: | :---: |
| ![SW-P01](./SW-P01.svg) | ![SW-P02](./SW-P02.svg) | ![SW-P03](./SW-P03.svg) |

---

## CAD / CAM / Laser / CNC Router Notes

1. **Zero open contours or stacked duplicate segments:** Every `.svg` file uses a single boolean-validated compound `<path fill-rule="evenodd">` composed strictly of analytical circular `A` arcs and `L` segments. Every `-R2010.dxf` file separates `OUTER_PROFILE` (Layer 1) from `INNER_APERTURE` cutouts (Layer 2) using native `CIRCLE` primitives and closed `LWPOLYLINE` entities with exact chord-bulge arcs (`bulge = tan(sweep / 4)`).
2. **Structural web margins:** At a `560 mm x 560 mm` (`22 in` to `24 in`) decorative screen scale, minimum structural bridge widths span `30.56 mm` (`1.203 in`) to `34.45 mm` (`1.356 in`), well above the `3.81 mm` (`0.150 in`) router floor for architectural plywood, MDF, acrylic, and aluminum sheet.
3. **Deterministic regeneration:** Run `python build_solwright_sampler.py` (requires `sympy`, `shapely`, `ezdxf`) to rebuild all `.svg` and `-R2010.dxf` files and run `ezdxf.audit()` verification (`0` errors).

## License

Code in `build_solwright_sampler.py` is released under the `MIT` License; vector and CAD sampler panels (`SW-P01`, `SW-P02`, `SW-P03`) are released under `CC-BY-4.0` / `MIT` for free personal and commercial evaluation (`$0.00`).

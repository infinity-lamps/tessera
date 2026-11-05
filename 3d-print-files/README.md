# 3D print files

Replacement parts for Tessera lamps, as STEP files. If a part cracks or goes
missing, print a new one here rather than replacing the lamp.

Everything marked `[TBC: ...]` still needs filling in before this page is final.

---

## Finding the right files

Each lamp has its own folder, named by edge length and then shape, the same
way the lamps are named:

```
3d-print-files/
  100mm-rhombic-dodecahedron/
    hub-3-valent.step
    hub-4-valent.step
    strut.step
    ...
  jigs/
    solder-jig.step
    glue-jig.step
```

The edge length and shape are on the label under your lamp. A part from one
folder will not fit a lamp of a different size or shape.

STEP files open in most CAD programs and slicers (PrusaSlicer, OrcaSlicer,
Bambu Studio, Cura). Use **Download** on the
[landing page](https://infinity-lamps.github.io/tessera/#parts), or the
download button on GitHub's file page.

## Before you print

- **Print one of each first.** Print a single strut, cap and hub, check they
  fit together, and check that they fit your lamp, before printing a full set.
  Printers differ, and a small dimensional error multiplies across every joint.
- **Match the colour.** The inside of the frame should be matte black. Any
  shine inside the lamp shows up as stray reflections and spoils the infinity
  effect.

## Default print settings

These apply to every part unless the part's own row below says otherwise.

| Setting | Value | Why |
|---|---|---|
| Material | PETG | Copes with the warmth from the LEDs better than PLA |
| Colour | Matte black | Keeps reflections inside the lamp clean |
| Nozzle | `[TBC: 0.4 mm]` | |
| Layer height | `[TBC: mm]` | |
| Walls / perimeters | 3 or more | Strength at the joints |
| Top / bottom layers | `[TBC]` | |
| Infill | `[TBC: % and pattern]` | |
| Supports | `[TBC: none / build plate only]` | |
| Bed adhesion | `[TBC: brim / none]` | |
| Nozzle temperature | `[TBC: °C]` | Use your filament maker's range |
| Bed temperature | `[TBC: °C]` | |

Tested on: `[TBC: printer and slicer]`.

## Parts

### `[TBC: edge length and shape, e.g. 100 mm rhombic dodecahedron]`

Folder: `[TBC: folder name, e.g. 100mm-rhombic-dodecahedron]`

| Part | File | Number in one lamp | Print orientation | Supports | Notes |
|---|---|---|---|---|---|
| Strut | `strut.step` | `[TBC]` | `[TBC]` | `[TBC]` | One per edge; the LED channel faces into the lamp |
| Snap cap | `[TBC].step` | `[TBC]` | `[TBC]` | `[TBC]` | Clips over each strut |
| Hub, 3-way | `hub-3-valent.step` | `[TBC]` | `[TBC]` | `[TBC]` | Corners where three edges meet |
| Hub, 4-way | `hub-4-valent.step` | `[TBC]` | `[TBC]` | `[TBC]` | Corners where four edges meet |
| Panel template | `[TBC].step` | 1 | Flat | None | A guide for cutting a replacement face. Not part of the lamp |

Copy this section for each lamp size and shape you publish.

### Assembly jigs (kits only)

Folder: `jigs`

| Part | File | Number needed | Print orientation | Supports | Notes |
|---|---|---|---|---|---|
| Solder jig | `solder-jig.step` | 1 | `[TBC]` | `[TBC]` | Holds the LED strip in place while soldering |
| Glue jig | `glue-jig.step` | 1 | `[TBC]` | `[TBC]` | Holds a hub and strut square while the glue sets |

## Fitting a replacement part

`[TBC: short steps, or a link to the relevant section of the User Guide or Kit
Build Guide in ../guides/]`

## Licence

These files are licensed under
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/): you can print,
share and adapt them, with credit, under the same terms. See
[LICENSE-CONTENT](../LICENSE-CONTENT).

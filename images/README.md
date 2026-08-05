# images/

Drop image files here using these exact names — `index.html` already points at them.
Any figure whose file is missing renders a visible dashed placeholder naming the file,
so nothing goes silently blank.

| File | What it should show | Priority |
|---|---|---|
| `hero-cutlass.jpg` | Cover shot — the Cutlass, wide | **Critical** |
| `actuation-assembly.jpg` | SolidWorks isometric render, full assembly | **Critical** |
| `actuation-drawing.jpg` | One released drawing sheet, title block visible | **Critical** |
| `foosball-gdt.jpg` | Part drawing with GD&T callouts and fit dimensions readable | **Critical** |
| `foosball-assembly.jpg` | Full 22-component assembly render | High |
| `actuation-motion.jpg` | Motion study output — force vs. time plot | High |
| `moto-exhaust.jpg` | The fabricated exhaust, installed | High |
| `moto-harness.jpg` | RPM gauge wired into the stock harness | High |
| `foosball-section.jpg` | Assembly drawing, section view + BOM | Medium |
| `shop-parts.jpg` | Six machined parts laid out, one overhead shot | Medium |
| `cutlass-engine.jpg` | Engine work | Medium |
| `cutlass-intake-carb.jpg` | Intake manifold and carburetor | Medium |
| `cutlass-drum-brake.jpg` | Drum brake rebuild | Medium |
| `cutlass-floorpan.jpg` | Floor pan replacement | Medium |
| `cutlass-full.jpg` | The car as it stands | Medium |
| `moto-xr200.jpg` | Honda XR200 | Medium |
| `moto-sr50.jpg` | Aprilia SR50 | Medium |
| `moto-road.jpg` | Bike on the road | Low |
| `clock-build.jpg` | Assembled alarm clock | Low |
| `clock-wiring.jpg` | Circuit layout / wiring | Low |
| `shop-lathe.jpg` | Lathe or mill setup mid-operation | Low |

**Quality notes.** CAD renders beat screenshots — plain background, or just RealView.
Crop so the model fills the frame; nobody needs to see the FeatureManager tree. Export
drawing sheets to PNG at high DPI so GD&T callouts stay legible when zoomed. Resize
photos to ~1600px wide before uploading — full-size phone photos make the page crawl.

**If a photo doesn't exist**, delete that `<figure>` block in `index.html` rather than
shipping the placeholder. Two good images beat three with a hole.

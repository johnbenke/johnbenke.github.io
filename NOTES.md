# Open items

The site is public, so unanswered questions live here rather than as visible
boxes on the page. Everything currently on `index.html` traces to
`John_Benke_Engineering_Portfolio.docx` or `John_Benke_Master_File.docx` —
nothing was invented. These are the gaps.

## Questions for John

Carried over from the `>> NEEDED FROM JOHN` markers in the portfolio doc, plus
a few the site itself raised.

**Individual contribution.** Three team projects currently describe the team's
work with no split called out, because the source docs don't have one. The
foosball table does (player geometry, assembly integration, report sections) and
reads much stronger for it. Needed for:
- Multi-Mechanism Actuation System (MEMS 3110) — which bullets were yours?
- AF16 Heat Transfer (MEMS 3420) — the meshing, the analytical fin area, the validation write-up?
- HVAC Cooling Load (MEMS 3430) — load calculation, cycle model, refrigerant study, or the financial/environmental extension?

**What was the actuation mechanism actually for?** The write-up describes a
payload and a simulated occupant but never names the application. One plain
sentence would make that project far more readable.

**How were the worn piston rings confirmed?** Compression test, leak-down,
visual on teardown? Naming the test turns a claim into a method.

**Hours logged on the two bikes?** The Cutlass has 100+ documented hours and
that number carries weight on the page — a comparable figure would help.

**Code excerpts.** Two would materially strengthen the page:
- 5–10 lines of the CoolProp state-point solver from the HVAC project
- the alarm-clock sketch, e.g. the alarm-check loop

**Phone number.** The résumé carries `(914) 574-7347`. It is deliberately *not*
on the site — a public page gets scraped in a way a PDF sent to one recruiter
does not. Email and LinkedIn are there instead. Say the word and it goes on.

**Résumé PDF.** Not linked yet. Drop `resume.pdf` in the repo root and add a
link to the contact list in the masthead.

## Decisions already made

**BR+A internships are off the site.** Both source documents deliberately
exclude them, and `PORTFOLIO_SETUP.md` is explicit that no BR+A material goes
here without written permission. Worth knowing this cuts two summers of real
engineering experience from the page — it is on the résumé and LinkedIn, which
is where a recruiter will find it. Revisit only with permission.

**Skills traceability.** Revit, Bluebeam Revu and Newforma came from BR+A and
have no project on this page backing them, so they are not in the skills list.
ASHRAE 55 / 90.1 stayed because the MEMS 3430 project uses them directly.

**Project order.** The site leads with mechanism design and analysis rather
than the Cutlass, which is how the portfolio doc opens. For an engineering
application the CAD and simulation work should be the first thing read; the
restoration projects are still prominent, just lower.

## Images

Nine photos were extracted from the portfolio `.docx`, EXIF-rotated, resized to
max 1600px and written to `images/`. All are placed and captioned.

Still missing — every CAD and simulation visual. These are the highest-value
additions left, in order:

| File | Project | What it should show |
|---|---|---|
| `actuation-assembly.jpg` | MEMS 3110 | SolidWorks render, ideally the four states side by side (closed, open, extended, lowered) |
| `actuation-drawing.jpg` | MEMS 3110 | One released drawing sheet, title block and BOM visible |
| `actuation-motion.jpg` | MEMS 3110 | SolidWorks Motion force-vs-time plot (~207 lbf peak) |
| `comsol-temp-field.jpg` | MEMS 3420 | COMSOL temperature contour of the finned cylinder — the single best visual from that project |
| `comsol-mesh-convergence.jpg` | MEMS 3420 | Mesh convergence plot across the five refinement levels |
| `hvac-cycle-diagram.jpg` | MEMS 3430 | P-h or T-s diagram from the Python model |
| `hvac-load-breakdown.jpg` | MEMS 3430 | Cooling load breakdown (solar 53.1 / conduction 21.7 / equipment 20.8 / metabolic 4.4) |
| `foosball-gdt.jpg` | MEMS 202 | Part drawing with GD&T callouts legible |
| `foosball-assembly.jpg` | MEMS 202 | Full 22-component assembly render |
| `shop-parts.jpg` | MEMS 1001 | Six machined parts laid out, one overhead shot |
| `clock-build.jpg` | Circuits | The finished clock and/or breadboard wiring |

Figures are only added to `index.html` once the file exists — a missing image
removes its own figure rather than showing a broken frame, so nothing on the
live page ever looks unfinished.

**Quality notes.** CAD renders beat screenshots; crop so the model fills the
frame. Export drawing sheets at high DPI so GD&T callouts stay legible zoomed.
Resize photos to ~1600px before committing.

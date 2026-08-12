# Open items

The site is public, so unanswered questions live here rather than as visible
boxes on the page. Everything on `index.html` traces to one of the source
documents — the two `.docx` files or the three project reports (MEMS 3110
design report, MEMS 3420 COMSOL report, MEMS 3430 thermal systems report).
Nothing was invented.

---

## ⚠ One thing to fix on the résumé and portfolio doc

**The IEC standards claim is not supported by the report.** Both documents say
the MEMS 3110 team "researched applicable safety standards (IEC 60825-1,
IEC 62133-2) to set the design envelope."

Section 2.3 of the design report is unedited instructor template text. It opens
*"Yep, you'll find codes & standards too. I'm leaving these two standards so
that you can see what the sections will look like,"* and both subsections
contain the same paragraph about laser radiation and a **golf striker design** —
boilerplate from a different example project. IEC 60825-1 covers laser products
and IEC 62133-2 covers portable batteries; the GASP has neither.

It has been **removed from the site** — from the project page and from the
skills list. Recommend cutting it from the résumé and
the portfolio doc too. An interviewer who asks "how did laser safety apply to a
wooden armoire?" gets nothing, and that costs more than the line is worth.

---

## Still needed from John

**Individual contribution on the three team projects.** Still the biggest gap.
None of the three reports splits the work by author, so the site describes team
output without naming John's part. The foosball entry does name it and reads
noticeably stronger. Needed for:
- **MEMS 3110 (GASP)** — team: Stephen Bell, John Benke, Eli Beauchamp. Whose were the drawing sheets, the Motion study, the linkage trigonometry, the operator's manual?
- **MEMS 3420 (COMSOL)** — team: John Benke, Emmanuel Jenkins, Chloe Lippert, Nate Smith. The meshing, the analytical fin area, the validation write-up?
- **MEMS 3430 (HVAC)** — team: John Benke, Danny Bruns, Anthen Primus, Susanna Yeh. The load calculation, the cycle model, the refrigerant study, the financial/environmental extension?

**How were the worn piston rings confirmed?** Compression test, leak-down, or
visual on teardown? Naming the test turns a claim into a method.

**Hours logged on the two bikes?** The Cutlass has 100+ documented hours and
that number carries weight on the page.

**Was the riding photo taken before or after the rebuild?** It now leads the
motorcycles page with a deliberately neutral caption ("The XR200 under power").
If it is post-rebuild, the caption should say so — that turns a nice photo into
evidence the work succeeded.

**The Arduino sketch.** The HVAC project now shows real code on the site and it
lifts that section; the alarm clock has no code and no photo, so it is the
weakest entry on the page. Even the alarm-check loop would help.

**Photos still missing.** Three projects have no image, so their cards on the
home page use a typographic tile instead of a photo. In priority order:

| Card | What would fill it |
|---|---|
| Alarm Clock | The breadboard/LCD photo — it exists, it just has not reached the repo yet |
| Foosball (MEMS 202) | One drawing sheet with GD&T callouts legible, or the 22-component assembly render |
| Machine Shop (MEMS 1001) | The six parts laid out on a plain surface, one overhead shot |

**Getting images in.** Pasting a photo into chat does not put a file on disk —
only documents do. Two routes that work: wrap the photos in a PDF or Word doc
and send that (this is how `moto-riding.jpg` arrived), or upload straight to
`images/` through the GitHub web UI. iCloud share links are blocked by the
sandbox proxy and cannot be fetched.

**Wainwright Building photo — provenance unconfirmed.** A photo was supplied
for the HVAC project but is being held out of the repo pending an answer. At
386x518 it is web-thumbnail size rather than phone-camera size, which suggests
it was downloaded rather than taken. The building photo in the MEMS 3430 report
was excluded for the same reason. If John took it, it goes straight in; if not,
Wikimedia Commons has freely licensed photographs of the Wainwright that can be
used with attribution.

The typographic tiles look deliberate rather than broken, so there is no rush —
but a photo beats a number on a card every time. Drop the file in `images/`,
crop to 3:2, name it `thumb-<slug>.jpg`, and swap the `<div class="stat">` in
`index.html` for an `<img class="thumb" src="images/thumb-<slug>.jpg" alt="">`.

**Résumé PDF.** Not linked. Drop `resume.pdf` in the repo root and add it to the
contact list in the masthead of `index.html`.

**Phone number.** The résumé carries `(914) 574-7347`; it is deliberately *not*
on the site, since a public page gets scraped in a way a PDF sent to one
recruiter does not. Email and LinkedIn are there. Say the word and it goes on.

---

## Answered by the three reports

- **What the MEMS 3110 mechanism was for** — the Ghost Armoire Set Piece
  (G.A.S.P.), a stage mechanism for *A Christmas Carol*: the Ghost of Christmas
  Past levitates out of a cabinet and descends to the stage, driven entirely by
  stagehands through cords, torsion springs and a three-bar linkage. Client was
  Prof. Rob Mark Morgan, interviewed 25 March 2026. This was the single biggest
  gap on the page and it is now the strongest story on it.
- **Python code excerpt** — the CoolProp refrigerant loop is on the site.
- **Fin effectiveness (20.7) and efficiency (98.7%)** — neither was in the
  résumé or portfolio doc; both are now on the page.
- **Mesh convergence numbers** — 1,573 → 96,089 elements, <0.27% variation.
- **Full refrigerant comparison** — all five fluids with mass flow, compressor
  power and COP, now a table rather than one recommended value.

## Images

**From the portfolio `.docx`** (9): hero, five Cutlass, three motorcycle.

**From the project reports** (18): GASP renders (doors open, platform extended,
lowered), four released drawing sheets, the BOM sheet, the labeled component
view, the Motion force plot and both door-force plots; the COMSOL temperature
field, mesh, CAD half-model and cut-line plot; the HVAC cycle schematic and
T–s diagram.

All EXIF-rotated where needed, resized to max 1600px, saved as progressive JPEG.

Two figures were deliberately **not** used: the Wainwright Building photograph
from the MEMS 3430 report (sourced from elsewhere — not John's work, unclear
rights) and the *A Christmas Carol* production still from the MEMS 3110 report
(same reason).

A figure whose image file is missing removes itself rather than showing a broken
frame, so no page ever looks half-finished — but a typo in a filename fails
silently. Check the page after adding one.

## Theme

Muscle car, not drafting office — in a cool key. Cool off-white ground with a
faint blue lean, pinstripe blue, violet, and an ice hairline, with hand-laid
pinstriping as the organising motif.

- **Pinstripes.** A triple coach line — heavy stroke, contrast hairline, closing
  hairline — drawn in pure CSS gradients, no images. It appears on:
  the masthead divider; under every section heading; across the top *and* foot
  of every card; down both flanks of the page as fixed body-side stripes
  (`.sidepin`, hidden below 1080px where there is no room); trailing out to the
  margin from every subsection label; the left edge of metric tiles, code blocks
  and figure captions; under table headers; and closing the footer and
  prev/next rail. Cards invert theirs blue↔violet on hover.
- **Badge type.** The name is heavy italic uppercase, like body-side badging.
  Project titles are tight bold sans; every label is letterspaced uppercase.
- **Colour has jobs.** Blue carries section headings, "read more" and
  odd-numbered metric tiles; violet carries kickers, skill labels, table headers
  and tool chips; the ice tone is only ever a caption rule. Stripes read
  blue-dominant with violet as the inner line, and invert on hover.
- **Chrome trim.** 2px ink borders on cards, figures, tables and code blocks —
  which in dark mode invert to near-white and read as brightwork.
- The grain from the earlier theme survives at ~14% — lower than on the warm
  ground, where it read as noise rather than texture.

The earlier drafting-manual treatment (title blocks, sheet numbers, plate tabs,
typewriter labels) was removed — see git history if it is ever wanted back.


## Structure

The site is a card grid (`index.html`) over eight project pages, all sharing
`style.css`. Each project has its own URL, so a single project can be sent to a
company directly. See `PORTFOLIO_SETUP.md` for the page-to-project map.

---

## Decisions already made

**BR+A internships are off the site.** Both source documents deliberately
exclude them, and `PORTFOLIO_SETUP.md` is explicit that no BR+A material goes
here without written permission. This does cut two summers of real engineering
experience from the page — it is on the résumé and LinkedIn, which is where a
recruiter will find it. Revisit only with permission.

**Skills traceability.** Revit, Bluebeam Revu and Newforma came from BR+A and
have no project on this page backing them, so they are not in the skills list.
ASHRAE 55 / 90.1 stayed because the MEMS 3430 project uses them directly. The
IEC standards are gone for the reason above.

**Project order.** Card order, set by John: Cutlass → motorcycles → GASP →
COMSOL → HVAC → alarm clock → foosball → machine shop. The restoration work
leads, which also puts the three strongest photographs in the first two tiles;
the three projects with no photo fall to the end, so the typographic tiles sit
together rather than interrupting the grid. Prev/next links on the project
pages follow the same order — change one and change the other, or the walk
through the projects stops matching the grid.

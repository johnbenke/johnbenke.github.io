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

It has been **removed from the site**. Recommend cutting it from the résumé and
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

**The Arduino sketch.** The HVAC project now shows real code on the site and it
lifts that section; the alarm clock has no code and no photo, so it is the
weakest entry on the page. Even the alarm-check loop would help.

**Photos still missing:** the six machined parts from MEMS 1001 (lay them out,
one overhead shot), and the finished alarm clock / breadboard wiring. These are
the only two projects on the site with no visual at all.

**Résumé PDF.** Not linked. Drop `resume.pdf` in the repo root and add it to the
contact list in the masthead.

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
frame, so the live page never looks half-finished — but a typo in a filename
fails silently. Check the page after adding one.

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

**Project order.** The site leads with mechanism design and analysis rather than
the Cutlass, which is how the portfolio doc opens. For an engineering
application the CAD and simulation work should be read first; the restoration
projects are still prominent, just lower.

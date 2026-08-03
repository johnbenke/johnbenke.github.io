# John Benke — Portfolio Site

Single-file static site. Nothing to build, nothing to install.

---

## 1. Before you publish — three things

**a) Fill the TODO block.**
`index.html` has one red dashed `.todo` box in the MEMS 3110 project. Trossen's guide explicitly asks for *"detailed descriptions of your projects and your specific contributions, especially if it was a team effort."* Write 2–3 sentences on what was yours, then delete the `<div class="todo">…</div>` entirely.

**b) Drop in the remaining images.** Nine photos from your portfolio doc are already in `images/` and wired up — the cover shot, five Cutlass images, three motorcycle images. What's still missing is every CAD/simulation visual. Any figure without an image shows a dashed placeholder naming the file it wants, visible to anyone who opens the page, so fill them or delete those `<figure>` blocks.

**c) Nothing from BR+A goes on this site.** No healthcare project names, no Revit screenshots, no submittals, no shop drawings. Client-confidential. The site intentionally contains zero BR+A material — keep it that way unless you get written permission.

---

## 2. Deploy on GitHub Pages (free, ~10 minutes)

1. Create a GitHub account if you don't have one. **Pick the username carefully — it becomes your URL.** `johnbenke` → `johnbenke.github.io`.
2. Create a new **public** repository named exactly `<username>.github.io`.
3. Upload `index.html` and the `images/` folder to the repo root (drag-and-drop works: *Add file → Upload files*).
4. Go to **Settings → Pages**. Under *Source*, pick **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. Wait 1–2 minutes. Your site is live at `https://<username>.github.io`.

**Optional custom domain (~$12/yr, looks better on a resume):**
Buy `johnbenke.com` from Cloudflare or Namecheap → in Settings → Pages, enter it under *Custom domain* → add the DNS records GitHub shows you at your registrar → tick **Enforce HTTPS**.

### Faster alternative
If GitHub feels like a detour, **Carrd** ($19/yr) or **Google Sites** (free) will host the same content with a visual editor. The URL is what matters to the application form. GitHub Pages is worth the extra 20 minutes because the repo itself reads as a signal to an engineering hiring manager — but a live Google Site beats a perfect GitHub site you didn't finish.

---

## 3. Images to add

Put these in `images/`. Exact filenames — the HTML already points at them.

### Already in place
`hero-cutlass.jpg` · `cutlass-engine.jpg` · `cutlass-intake-carb.jpg` · `cutlass-drum-brake.jpg` · `cutlass-floorpan.jpg` · `cutlass-full.jpg` · `moto-xr200.jpg` · `moto-sr50.jpg` · `moto-road.jpg`

### Still needed

| File | What it should show | Priority |
|---|---|---|
| `actuation-assembly.jpg` | SolidWorks isometric render, full assembly | **Critical** |
| `actuation-drawing.jpg` | One released drawing sheet, title block visible | **Critical** |
| `foosball-gdt.jpg` | Part drawing with GD&T callouts and fit dimensions readable | **Critical** |
| `foosball-assembly.jpg` | Full 22-component assembly render | High |
| `actuation-motion.jpg` | Motion study output — force vs. time plot | High |
| `foosball-section.jpg` | Assembly drawing, section view + BOM | Medium |
| `shop-parts.jpg` | Six machined parts laid out on a plain surface, one overhead shot | Medium |
| `clock-build.jpg` | Assembled alarm clock | Low |
| `clock-wiring.jpg` | Circuit layout / wiring | Low |
| `shop-lathe.jpg` | Lathe or mill setup mid-operation | Low |
| `moto-exhaust.jpg` | The fabricated exhaust, installed | High |
| `moto-harness.jpg` | RPM gauge wired into the stock harness | High |

The three marked **Critical** are the ones Trossen's guide asks for by name — CAD screenshots. Without at least those, the page leads with two empty boxes.

**Quality notes.** CAD renders beat screenshots — use SolidWorks *Tools → Options → Document Properties* with a plain background, or just RealView. Crop screenshots so the model fills the frame; nobody needs to see your FeatureManager tree. For drawing sheets, export to PNG at high DPI so the GD&T callouts are actually legible when zoomed. Resize photos to ~1600px wide before uploading — full-size phone photos will make the page crawl.

**If a photo doesn't exist**, delete that `<figure>` block rather than shipping the placeholder. Two good images beat three with a hole.

---

## 4. Applying to Trossen

The form has separate required fields:

- **Direct Portfolio Link URL** → your live site URL
- **LinkedIn URL** → `https://www.linkedin.com/in/john-benke`
- **File upload** → **PDF only.** Export the resume `.docx` to PDF before uploading.

The resume itself carries the portfolio URL on the contact line — update it to your real domain once the site is live.

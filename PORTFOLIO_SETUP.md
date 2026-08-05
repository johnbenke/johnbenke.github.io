# John Benke — Portfolio Site

Single-file static site. Nothing to build, nothing to install.

---

## 1. Before you publish — three things

**a) Fill the TODO block.**
`index.html` has one red dashed `.todo` box in the MEMS 3110 project. Trossen's guide explicitly asks for *"detailed descriptions of your projects and your specific contributions, especially if it was a team effort."* Write 2–3 sentences on what was yours, then delete the `<div class="todo">…</div>` entirely.

**b) Drop in the images.** `images/` is currently **empty** — no photos were ever uploaded to the repo, so every figure on the page is a placeholder right now. `images/README.md` lists all 21 filenames the HTML points at, in priority order. Any figure without an image shows a dashed placeholder naming the file it wants, visible to anyone who opens the page, so fill them or delete those `<figure>` blocks.

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

The full list — 21 filenames, what each should show, priority order, and quality notes — lives in **`images/README.md`**. The exact names matter; the HTML already points at them.

Start with the four marked **Critical**: `hero-cutlass.jpg`, `actuation-assembly.jpg`, `actuation-drawing.jpg`, `foosball-gdt.jpg`. The three CAD ones are what Trossen's guide asks for by name. Without them the page leads with empty boxes.

---

## 4. Applying to Trossen

The form has separate required fields:

- **Direct Portfolio Link URL** → your live site URL
- **LinkedIn URL** → `https://www.linkedin.com/in/john-benke`
- **File upload** → **PDF only.** Export the resume `.docx` to PDF before uploading.

The resume itself carries the portfolio URL on the contact line — update it to your real domain once the site is live.

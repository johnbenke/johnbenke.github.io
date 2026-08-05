# John Benke — Portfolio Site

Single-file static site. Nothing to build, nothing to install.

---

## 1. Status

The site is **live** at https://johnbenke.github.io with the full content of
`John_Benke_Engineering_Portfolio.docx` — eight projects, the technical skills
summary, and coursework. The nine photos embedded in that document were
extracted and are in `images/`.

**What's still open** is tracked in [`NOTES.md`](NOTES.md): individual-contribution
splits on three team projects, a few method details, and every CAD/simulation
visual. Read that file before editing the page.

**Nothing from BR+A goes on this site.** No healthcare project names, no Revit
screenshots, no submittals, no shop drawings. Client-confidential. The site
intentionally contains zero BR+A material — keep it that way unless you get
written permission.

---

## 2. How it deploys

The repo is public and Pages is set to **GitHub Actions** as its source.
`.github/workflows/pages.yml` publishes the repo root as-is — no build step — on
every push to `main`. Push a change, wait a minute, the site updates.

To edit without a local clone: open a file on github.com, click the pencil,
commit to `main`. That's the whole loop.

**Optional custom domain (~$12/yr, looks better on a resume):**
Buy `johnbenke.com` from Cloudflare or Namecheap → in Settings → Pages, enter it
under *Custom domain* → add the DNS records GitHub shows you at your registrar →
tick **Enforce HTTPS**.

---

## 3. Adding images

Drop the file in `images/`, then add a `<figure>` to the matching project in
`index.html`. [`NOTES.md`](NOTES.md) lists which visuals are still missing and
what each should show, in priority order.

A figure whose image file is missing removes itself rather than showing a broken
frame, so the live page never looks half-finished — but that also means a typo in
a filename fails silently. Check the page after adding one.

Resize photos to ~1600px wide before committing. Export drawing sheets at high
DPI so GD&T callouts stay legible when zoomed.

---

## 4. Applying to Trossen

The form has separate required fields:

- **Direct Portfolio Link URL** → your live site URL
- **LinkedIn URL** → `https://www.linkedin.com/in/john-benke`
- **File upload** → **PDF only.** Export the resume `.docx` to PDF before uploading.

The resume itself carries the portfolio URL on the contact line — update it to your real domain once the site is live.

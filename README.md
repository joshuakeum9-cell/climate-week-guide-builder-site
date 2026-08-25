# Climate Week Guide Builder - documentation site

A single static page documenting the `climate-week-guide-builder` plugin: what it is, how the
pipeline runs, what a chapter lead has to do at each step, and what comes out the other end.

Audience is a Climate Tech Cities chapter lead who has just installed the plugin and has never
run it, plus whoever needs a reference when a run goes sideways.

## Files

```
index.html    the whole site, self-contained
.nojekyll     stops GitHub Pages running the file through Jekyll
README.md     this file
GAPS.md       what I needed and did not have, and the one factual conflict in the brief
```

No build step, no dependencies, no backend, no analytics. The only external request is the
Google Fonts stylesheet for Inter and Geist Mono.

## Local preview

Any static server will do. From this folder:

```bash
python -m http.server 8931
```

Then open `http://localhost:8931`. Opening `index.html` directly off the filesystem also works,
since nothing on the page depends on an origin.

## Deploy

**GitHub Pages.** Push this folder as the repository root, then Settings > Pages > Deploy from a
branch, root folder. The `.nojekyll` file is already present. Nothing else is required.

**Vercel.** Import the repository and accept the defaults. Framework preset "Other", no build
command, output directory `.`.

Both serve the page as-is.

## Design

Built on the Mintlify design system, matching the CTC chapter launch workflow site so the two
read as one family: Inter and Geist Mono, white canvas, hairline 12px cards, black pill buttons,
mint `#00d4a4` accent, sky-gradient hero, dark teal band, orange statement card.

The pipeline stepper is the hero element. Steps that need a human are visually distinct from
automated ones, and Stage 1b, the one hard gate, gets its own node treatment and a full band.

Verified in-browser: no console errors, no horizontal overflow at 375px or 1280px, the pipeline
stays a single vertical stack on mobile, the wide evidence table scrolls inside its own
container, one `h1` with a clean heading outline, `nav` / `main` / `footer` landmarks, no broken
anchors, and text contrast at or above 4.5:1 throughout. The orange statement card sits at
3.28:1, which clears the 3:1 large-text threshold and matches the existing component on the
reference site.

## Content rules this page follows

- Nothing fake. Every claim traces to a `SKILL.md` or reference file in the plugin.
- The plugin runs in Claude Cowork, not in chat. Stated in three places on the page.
- Sample guide links carry counts verified by fetching the live posts, not from memory.
- No invented metrics, timings, screenshots, or example output.
- No em dashes, per house style. Spaced hyphens instead.
- Sentence case headings.
- No "get started" CTA implying a signup. This is internal tooling.
- No Airtable base IDs and no personal profile URLs.

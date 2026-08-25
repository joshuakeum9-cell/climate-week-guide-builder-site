# What I needed and did not have

Per the brief's third deliverable. Nothing here blocked the build. Items 1 and 2 are the ones
worth a decision from you.

## 1. "Nine stages" conflicts with the table underneath it

The brief's section 4 opens with "Nine stages", then gives a table with **twelve rows**
(0, 0b, 1, 1b, 1c, 1d, 1e, 2, 3, 4, 5, 6). The plugin's own `ctc-climate-week-guide/SKILL.md`
describes the system as **seven stages**, with 0b, 1b, 1c, 1d and 1e as sub-steps hanging off
them.

Nine matches neither. I rendered all twelve rows and described it as **"Seven numbered stages,
twelve steps in all"**, which is true against both the table and the SKILL.md. The hero says
"7 of 12 steps" need you, counted off the Human column.

If you want a different framing, it appears in three places: the hero stat, the pipeline
section's opening line, and the intro sentence above the stepper.

## 2. "Roughly an hour of your own attention"

Used exactly as you wrote it, since you supplied it. Flagging only because it is the one number
on the page I could not trace to a file in the plugin, and the brief's own rule is not to invent
timings. If it is a real estimate off past runs, it is fine as-is. Say the word if you want it
cut or softened.

## 3. No screenshots or example output

The brief forbids inventing them and I did not. So the page has no picture of a finished guide,
no shot of the Word document with its yellow placeholders, no shot of the Airtable form. It
carries the argument in prose and structure instead.

If you want any of these, they need to come from you as real image files:

- A page of a shipped guide as published on Substack
- The `.docx` open in Word, showing a category cover image and a yellow placeholder
- The published Airtable submission form

The one thing I could see wanting most is the before/after of a Substack paste: markdown showing
literal `##` characters next to the HTML paste rendering correctly. That is the page's most
useful practical tip and a screenshot pair would land it harder than the diagram I drew.

## 4. Two of the four shipped guides are now linked, two are not

RESOLVED IN PART. The "See a finished guide" block at the end of "What you get"
links the NY 2025 and NY 2024 posts, with counts verified by fetching both live
pages (2025: 506 events, 25 themes, 23,144 words, which matches the evidence
table exactly; 2024: 477 events, 24 themes). NY 2024 is labelled on the page as
sitting outside the plugin's four-guide reference set, because it does.

Still missing: canonical URLs for the London 2026, PNW 2026, and Chicago 2026
guides. Send them and I will link those rows of the evidence table too.

## 5. No install or "how do I get this plugin" section

The brief's content spec does not cover it, and it explicitly rules out a get-started CTA. So a
chapter lead who lands on this page and has *not* yet installed the plugin has no next step.
That may be deliberate, since the audience is defined as someone who has just installed it. If
you want a short install block, it needs the marketplace or repository install line.

## 6. Deployment not performed

I built the files and verified them locally. I have not created a repository, pushed anything, or
deployed to Pages or Vercel, since the brief asked for deployable static output rather than a
live deploy, and publishing is your call. `README.md` has the steps for both targets.

## 7. Per-stage timings

Not given, not invented, not shown. The page says a full run for a large city spans more than one
sitting, which is your line from the brief, and nothing more granular. If you have real numbers
from the four runs, the stepper has room for a duration on each step.

---

## Facts I verified against the plugin rather than taking on trust

All of these check out, so the page states them plainly:

- Eight skills in the plugin
- Eleven QA gates (Gates 1, 2, 3, 3b, 3c, 3d, 4, 5, 5b, 5c, 6)
- 26 category cover images, present as real `.png` files in the category-guide skill's assets
- Guide counts: London 1,000+/26, NY 506/25, PNW 277/22, Chicago 141/24
- 935 spaced hyphens in NY 2025 (also 82 PNW, 49 Chicago, 28 London, which I included since it
  strengthens the point)
- 23 MB of PNGs becoming about 2.3 MB of base64 at 800px
- The Chicago "26 Categories" vs 24 defect, and the "How to LCAW" leftover in a Chicago guide
- The `luma.com` origin requirement and the absence of any fallback
- Stage 1b not proceeding on silence, and the plugin refusing to recreate an existing base

The descriptive-vs-commentary before/after pair on the page is quoted from the real table in
`ctc-climate-week-category-guide/SKILL.md` rather than written to illustrate the rule.

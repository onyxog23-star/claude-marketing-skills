---
name: landing-page-builder
description: Build a single-file, conversion-focused landing page (HTML + inline CSS) from a short product brief. Use when asked for a landing page, sales page, waitlist page, launch page or "a page for my offer".
---

# Landing Page Builder

Turn a brief into a fast, responsive, self-contained landing page that is ready to deploy on GitHub Pages, Netlify or any static host.

## 1. Collect the brief

Before writing, make sure you have these. Ask only for what is missing, in one message.

| Field | Example |
|---|---|
| Product / offer | "LearnMizo – learn the Mizo language online" |
| Audience | "Diaspora parents who want their kids to speak Mizo" |
| Main outcome for the visitor | "Hold a simple conversation in 30 days" |
| Primary call to action | "Start free lesson" + destination URL |
| Proof you actually have | Real numbers, real quotes, logos (or "none yet") |
| Brand | Colours, fonts, tone (or "pick for me") |

If the user says "just build it", make sensible assumptions and list them at the top of your reply.

## 2. Write the copy first (before any HTML)

Follow the structure in `references/page-structure.md`. Rules:

- **Headline = outcome, not feature.** Max ~10 words. Test: would the audience say "yes, that's what I want"?
- **Subheadline** explains *how* in one sentence.
- **One primary CTA**, repeated (hero, mid-page, footer). Same wording every time.
- Benefits are written as "You can…" or "No more…", not as feature lists.
- **Never invent proof.** No fake testimonials, user counts, ratings or logos. If proof is missing, use a clearly marked placeholder: `<!-- TODO: add a real customer quote -->` and a visible "Your testimonial here" only in drafts.
- Keep reading level simple (aim for grade 6–8).

## 3. Build the page

Start from `assets/template.html` and replace the `{{placeholders}}`.

Technical requirements:
- Single file, all CSS inline in `<style>`; no frameworks. JavaScript only if needed (e.g. FAQ toggle).
- Mobile-first; test widths 360px, 768px, 1280px.
- Semantic HTML: one `<h1>`, sections with `<h2>`, `<main>`, `<footer>`.
- Fill in `<title>` (≤60 chars), `meta description` (≤155 chars), Open Graph tags.
- Colour contrast at least WCAG AA (4.5:1 for body text).
- Buttons ≥ 44px tall; CTA visible without scrolling on mobile.
- Images: use `loading="lazy"`, width/height set, descriptive `alt`.

## 4. Quality check before delivering

Run through `references/checklist.md` and fix anything that fails. Then deliver:
1. The HTML file.
2. A 3-line summary: headline chosen, CTA, assumptions made.
3. Two alternative headlines for A/B testing.

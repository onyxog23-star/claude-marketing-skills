---
name: seo-page-audit
description: Audit a single web page (URL or pasted HTML) for on-page SEO and conversion basics, then return a prioritised fix list with ready-to-paste titles, meta descriptions and headings. Use when asked to check SEO, audit a page, improve rankings, or review a landing page.
---

# SEO Page Audit

## Input
A URL (fetch it) or the page's HTML. Ask for the **target keyword** and **audience/country** if not given; otherwise infer the keyword from the page and say so.

## What to check

**Indexing & basics**
- `<title>` present, unique, 30–60 chars, keyword near the start
- Meta description 120–155 chars, includes keyword + a reason to click
- Canonical tag; no accidental `noindex`
- `lang` attribute, viewport meta, HTTPS

**Content structure**
- Exactly one `<h1>`, contains or reflects the keyword
- Logical H2/H3 order, no skipped levels used for styling
- Keyword and close variants used naturally in the first 100 words
- Thin content (< 300 words of real text on a page meant to rank)

**Links & media**
- Images: `alt` text present and descriptive; file size reasonable; width/height set
- Internal links to related pages; descriptive anchor text (not "click here")
- Broken links (if you can check them)

**Social & structured data**
- Open Graph title/description/image; Twitter card
- Relevant schema.org JSON-LD (Organization, Product, FAQPage, Article…)

**Conversion basics**
- Clear primary CTA above the fold
- Page states who it's for and what to do next

## Output format

1. **Score card** – a table: Area · Status (✅ / ⚠️ / ❌) · Note
2. **Top 5 fixes** ordered by impact ÷ effort
3. **Ready-to-paste fixes** – new title, meta description, H1, and any missing alt texts or JSON-LD
4. **What I couldn't check** – e.g. page speed, backlinks, Search Console data – and how to check them (PageSpeed Insights, Search Console)

Do not guess search volumes or rankings. If data isn't available, say so.

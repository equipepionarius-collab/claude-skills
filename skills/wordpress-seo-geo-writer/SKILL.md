---
name: wordpress-seo-geo-writer
description: Write a WordPress article optimized for SEO (Google) and GEO (being cited by AI search engines). Use when asked for an article, a blog post or web content to publish on WordPress.
---

# WordPress SEO + GEO writer

Produce a complete web article, ready to paste into WordPress, optimized both for Google rankings (SEO) and for citation by AI search engines (GEO: ChatGPT Search, Google AI Overviews, Perplexity).

## Step 1: frame the topic

Before writing, establish (ask only for what is missing and cannot be inferred):
- The **topic** and the **search intent** (informational, transactional, local).
- The **main keyword** and 3 to 6 **secondary keywords** or related queries.
- The **audience** (consumers, professionals) and the **location** if the topic is local.
- The target **length** (default 1,000-1,500 words) and the **tone**.

If the user gives no keywords, propose them from the topic. When a keyword tool is available (Semrush, Ahrefs, web search), use it to check volume and competition before writing. Otherwise say: "Check with a keyword tool before publishing."

## Step 2: structure for SEO

- **Title tag**: 60 characters max, main keyword first.
- **Meta description**: 140-160 characters, compelling, includes the main keyword.
- **URL slug**: short, lowercase, with the keyword, no stop words.
- **One H1** = the article title. Logical H2/H3 subheadings with secondary keywords where natural.
- **Intro**: answer the intent in the first 2-3 sentences.
- **Linking**: suggest 2-4 relevant internal links (placeholders if exact URLs are unknown) and 1-2 external links to authoritative sources.
- **Density**: main keyword used naturally, never stuffed.
- **Alt text**: a descriptive alt attribute for each suggested image.

## Step 3: optimize for GEO (AI citations)

AI engines cite content that is **factual, structured and directly answering**. So:
- Open each section with a **self-contained answer sentence** (a clear, quotable claim that makes sense out of context).
- Prefer **lists, tables and definitions** to long paragraphs.
- Include **concrete data** (numbers, timeframes, steps, thresholds) rather than generalities.
- Add an **FAQ section** (3-6 questions) using real user phrasing, with short direct answers.
- Cite **sources and dates** whenever a claim rests on verifiable facts.

## Step 4: structured data (JSON-LD)

Provide a `<script type="application/ld+json">` block to paste into the article:
- `Article` (headline, description, author, datePublished).
- `FAQPage` if there is an FAQ.
- `LocalBusiness` only if the topic is local and the details are known.

## Step 5: deliver

Default output: **a clean HTML file** (headings, `<p>`, `<ul>`, `<table>`, no inline styles) ready to paste into the WordPress editor, with at the top:
- Proposed title
- Meta description
- Proposed slug
- The JSON-LD block

End with a short pre-publish checklist: keywords to validate, internal links to fill in, image to add.

## Rules

- **Factual and honest** content: never invent statistics or quotes. Clearly mark what must be checked.
- Write for humans first; optimization must never hurt readability.
- Write in the language of the request.

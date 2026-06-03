# Apex Data Cloud — Site Implementation & SEO/GEO Guide

A complete, deploy-ready Jekyll site engineered for search (Google, Bing) and answer-engine (ChatGPT, Claude, Gemini, Perplexity) visibility. Push this folder to GitHub and serve via GitHub Pages.

---

## 1. What's in this repo

| Area | Files | Result |
|---|---|---|
| **Homepage** | `index.md` | Rebranded to **Apex Data Cloud**, title set to *"AI, Data Analytics & Machine Learning Consulting \| Apex Data Cloud"*, **bot removed**, now deep-links into every section page |
| **SEO infrastructure** | `_includes/head.html`, `schema-organization.html`, `schema-page.html`, `robots.txt`, `sitemap-index.xml`, `llms.txt` | Canonical, OG, Twitter, full JSON-LD graph, robots (incl. AI crawlers), sitemap index, RSS (`/feed.xml` via jekyll-feed), llms.txt |
| **Design system** | `assets/css/apex.css`, `_layouts/*`, `_includes/nav.html`, `footer.html`, `site-js.html` | Same navy + rose look, now shared across all pages |
| **10 service pages** | `services/*` | `/services/` hub + the 10 requested services |
| **6 industry pages** | `industries/*` | `/industries/` hub + 6 |
| **3 location pages** | `locations/*` | Local SEO (service-area model) |
| **4 assessments** | `assessments/*` | Lead-gen forms (Formspree) with `generate_lead` GA events |
| **Glossary / Comparisons** | `_glossary/*` (9), `_comparisons/*` (3) | GEO/citation content with `DefinedTerm` + comparison schema |
| **Blog / Case studies / Guides / Research** | `_posts/*` (3), `_case_studies/*` (2), `resources/*` | Seeded + index pages |
| **Backlog** | `CONTENT-STRATEGY.md` | 100 articles, 50 FAQs, 25 case studies, 25 comparisons, 25 glossary terms, prioritized |

**~60 indexable URLs today** (objective was 50+).

---

## 2. Before you deploy — REQUIRED

1. **Add the logo.** Drop `apex_logo.PNG` into the repo root (it's referenced site-wide but was not tracked in the source repo). Ideally also add a dedicated **`og-image.png` (1200×630)** for richer social/AI cards and set `image:` in `_config.yml` to it.
2. **Confirm the Formspree endpoint.** All forms post to `https://formspree.io/f/xqedrddj` (carried over from the original site). Verify it routes to the right inbox, or replace the ID in `_includes/contact-form.html` and `_includes/assessment-form.html`.
3. **Confirm the LinkedIn URL** in `_config.yml` (`company.sameAs`) — update or remove if the handle differs.
4. **Set the GitHub Pages source** to this folder's branch, with a custom domain `apexdata.cloud` (add a `CNAME` file containing `apexdata.cloud`).

## 3. Deploy

```bash
# from this folder
git init && git add . && git commit -m "Apex Data Cloud SEO/GEO site"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
# In GitHub: Settings → Pages → Build from branch (main) → custom domain apexdata.cloud
```

Local preview (optional, needs Ruby): `bundle install && bundle exec jekyll serve`.

## 4. After deploy

- Submit `https://apexdata.cloud/sitemap.xml` in **Google Search Console** and **Bing Webmaster Tools**.
- Request indexing of the homepage and `/services/`.
- Create/claim a **Google Business Profile** for the Orlando service area (strengthens local + the `LocalBusiness` schema).
- Verify rich results with Google's **Rich Results Test** (FAQ, Breadcrumb, Service should validate).

---

## 5. How the SEO/GEO system works

- **Entity consistency:** every page emits an `Organization` + `ProfessionalService/LocalBusiness` + `WebSite`/`SearchAction` graph (`schema-organization.html`) — one consistent "Apex Data Cloud" entity for Google's Knowledge Graph and AI systems.
- **Per-page schema** (`schema-page.html`) auto-generates `BreadcrumbList` on every page, plus `Service` (service pages), `FAQPage` (any page with `faqs:`), `Article` (posts/guides/case studies), and `DefinedTerm` (glossary) — all from front matter, no hand-coding.
- **GEO (AI citation) design:** TL;DR summary boxes, direct-answer FAQ blocks, definition/comparison pages, an `llms.txt`, and a robots.txt that explicitly allows GPTBot, ClaudeBot, PerplexityBot, Google-Extended, etc. These are the formats answer engines extract and cite.
- **Internal linking:** the homepage now links into every hub; services cross-link 3+ siblings; glossary ↔ comparisons ↔ services are densely interlinked; the `page` layout auto-adds a CTA + assessment sidebar on every content page.

### Adding new content (fast)
- **New service/page:** create a `.md` with `layout: page`, fill `title/description/eyebrow/faqs/related`. Schema + breadcrumb + CTA are automatic.
- **New glossary term:** add a file in `_glossary/` with `defines:` set.
- **New comparison:** add a file in `_comparisons/`.
- **New article:** add `_posts/YYYY-MM-DD-slug.md` with `layout: post`.

---

## 6. Prioritized roadmap

Scored on **Traffic impact / AI-search impact / Ease / Lead-gen impact** (H/M/L).

### Phase 1 — ship now (this repo) ✅
Homepage rebrand + title + bot removal, full schema/robots/sitemap/RSS, 10 services, 6 industries, 3 locations, 4 assessments, 9 glossary, 3 comparisons, seed blog/case studies/guides/research.
*Traffic: H · AI: H · Ease: done · Leads: H*

### Phase 2 — first 30 days (highest ROI)
1. **Add logo + og-image, submit sitemaps, claim Google Business Profile.** *T:H AI:M Ease:H Leads:M*
2. **Build the P1 glossary terms** (predictive analytics, machine learning, CDP, LTV, attribution, data pipeline, data warehouse, data governance) — fast, high AI-citation value. *T:M AI:H Ease:H Leads:L*
3. **Build the P1 comparisons** (GPT vs Claude vs Gemini, Snowflake vs Databricks, build vs buy, MTA vs MMM, AWS vs Azure vs GCP). *T:H AI:H Ease:M Leads:M*
4. **Publish 6–8 P1 blog articles** from Clusters A/B/C. *T:H AI:H Ease:M Leads:M*
5. **Add `faqs:` blocks** to remaining service/industry pages from the FAQ list. *T:M AI:H Ease:H Leads:L*

### Phase 3 — 60–90 days
6. Build remaining P1/P2 articles (target ~2–3/week) and 6–8 anonymized case studies. *T:H AI:M Ease:M Leads:H*
7. Add the remaining glossary + comparison pages (toward 25 each). *T:M AI:H Ease:M Leads:L*
8. Add Orlando/Florida local content + Google Business Profile posts; pursue local citations. *T:M AI:L Ease:M Leads:M*

### Phase 4 — ongoing
9. Refresh the AI-statistics research page with cited primary sources; publish an annual "State of Enterprise AI." *T:M AI:H Ease:L Leads:L*
10. Build genuine case studies with named clients (replace anonymized samples) — strongest conversion + trust signal. *T:M AI:M Ease:L Leads:H*

---

## 7. Notes & integrity
- **No fabricated data:** location pages use a service-area model (areaServed Orlando/Central FL/Florida) with no invented street address or phone. Case studies are clearly labeled **anonymized/representative**. The stats page ships with placeholders instructing you to add cited primary sources before external use.
- **Design preserved & extended:** the original navy + rose palette and components are intact; new pages reuse them via `assets/css/apex.css`.

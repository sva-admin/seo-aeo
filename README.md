# seo-aeo

A 9-phase, approval-gated SEO and AEO build for Next.js static sites that adds per-page metadata, JSON-LD, llms.txt, dynamic OG images, a tuned sitemap, and an AI-crawler allowlist.

An original skill by Silicon Valley Academy.

## What it does

SEO gets you into Google, Bing, and DuckDuckGo. AEO (AI Engine Optimization) gets you into ChatGPT, Claude, Perplexity, Gemini, and Copilot. The two stacks overlap heavily but ship different artifacts, and this skill ships both in one pass:

- Per-page metadata: title, description, canonical, hreflang, OpenGraph, Twitter cards
- Site-wide and per-page JSON-LD: Organization, WebSite, FAQPage, LocalBusiness
- `llms.txt` and `llms-full.txt` for AI engines
- A dynamic 1200x630 OpenGraph image built from your brand tokens
- A tuned sitemap with per-route priority and changefreq
- `robots.txt` with an explicit AI-crawler allowlist
- A deployment runbook a non-technical owner can operate after you leave

Every phase pauses for your approval, builds, and then verifies against the emitted HTML rather than the source. Nothing is marked done because the config looked right.

## Install

Paste this into Claude Code:

```
Install the seo-aeo skill from github.com/sva-admin/seo-aeo
```

Then invoke it in any session with `/seo-aeo`. The skill is a single self-contained file: no dependencies, no scripts, no external state.

## Usage

```
/seo-aeo                  # full 9-phase guided build with approval gates
/seo-aeo --auto           # confident defaults, minimal gates
/seo-aeo --phase <N>      # run only phase N (1 to 9)
/seo-aeo --audit          # read-only report, no changes
/seo-aeo --help           # print the usage block
```

Built for Next.js 14+ App Router with `output: 'export'` on Vercel. The final section of the skill covers adapting it to the Pages Router, SSR, Astro, Eleventy, and Hugo.

## Learn free

Learn free at https://loop.sv-academy.org/tutorials

---

More skills: https://github.com/sva-admin/claude-skills
Silicon Valley Academy: https://sv-academy.org

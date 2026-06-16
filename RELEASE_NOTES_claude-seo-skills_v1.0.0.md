# Growth Operating System v1.0.0

The first complete release. Twelve original, data-first Claude agent skills for SEO and growth. Where most SEO tooling optimizes for rankings, this suite optimizes for pipeline. Every skill reads real data from Ahrefs, Google Search Console, GA4, and Microsoft Clarity, takes Core Web Vitals from field data, and weighs decisions against the leads they produce.

Install the whole suite in Claude Code with two commands, or upload individual skills to Claude.ai using the bundles attached below.

## What's inside

Twelve skills, shipped as one plugin, `growth-os`, organized so they hand work to each other rather than sit as islands.

**Strategy**
- `cited-framework`: audits a brand across the five CITED layers (Citation Surface, Information Architecture, Technical Foundation, Evidence-Rich Extraction, Demand Capture) and runs the Citation Flywheel.
- `growth-audit`: revenue-weighted, full-funnel audit across Ahrefs, GSC, GA4, Clarity, Core Web Vitals, and lead data. Ranks findings by business impact, not severity.

**Foundation**
- `technical-foundation`: crawl, index, render, and Core Web Vitals from field data, with deploy-time drift checks. Programmatic checks included.
- `search-demand-map`: keyword, intent, SERP-feature, and topic-cluster mapping scored by lead value and buying stage, not raw volume.

**Content and experience**
- `content-engine`: gap analysis against real competitors, E-E-A-T and citability, publishing sequence by time-to-rank, and multimodal briefs.
- `search-experience`: SXO. Reads the SERP backward to catch page-type mismatch, derives the user stories behind a query, and scores the page per persona.
- `conversion-cro`: finds the friction between traffic and leads using GA4, Clarity, and CRM data, then prescribes specific UX, UI, and CRO fixes.

**AI search and structure**
- `ai-search-visibility`: get cited across AI Overviews, AI Mode, ChatGPT, Perplexity, Gemini, and Copilot. Citation share, extraction structure, entity signals, llms.txt, and tracking.
- `structured-data-engine`: JSON-LD, entity and knowledge-graph markup, and rich-result eligibility, matched to the SERP features worth winning.

**Authority and measurement**
- `authority-engine`: backlink profile, anchor health, toxic-link triage, competitor link gap, and a digital-PR plan led by original research.
- `competitive-intelligence`: competitor SEO, content, and SERP ownership, plus share of voice across classic and AI search.
- `growth-intelligence`: one reporting layer over Ahrefs, GSC, GA4, Clarity, and your CRM, tying rankings and traffic to leads and revenue.

## Install

### Claude Code (whole suite)

```bash
/plugin marketplace add avikbal-dm/claude-seo-skills
/plugin install growth-os@avikbal-growth-os
```

### Claude.ai (one skill at a time)

Download the `.skill` files attached to this release, open Settings > Capabilities > Skills, and upload the ones you want. Each file is a single skill.

### Claude Code or Desktop (manual)

```bash
git clone https://github.com/avikbal-dm/claude-seo-skills.git
cp -r claude-seo-skills/plugins/growth-os/skills/* ~/.claude/skills/
```

## A note on speed and on data

Search does not rank on a seven-day promise, and this suite does not pretend it does. Each module flags its quick wins with honest timeframes: days to weeks for technical unblocks, schema, and citation restructures, weeks for page-two pushes and comparison pages, weeks to months for authority and new content.

These skills encode a method, not a verdict. They assume access to the accounts they read, and they need your judgment on top. Treat projected outcomes as ranges.

Built by Avik Bal, author of *CITED: The Growth Operating System for AI Search*.

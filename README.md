# Growth Operating System for SEO, AEO, GEO, SXO

Original Claude agent skills that run SEO and growth off real data and actual leads. Where most SEO tooling optimizes for rankings, this suite optimizes for pipeline. Every skill pulls from Ahrefs, Google Search Console, GA4, and Microsoft Clarity, reads Core Web Vitals from field data, and weighs decisions against the leads they produce, not the vanity metrics they move.

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/status-stable-brightgreen)
![Modules](https://img.shields.io/badge/modules-12-blue)
![Claude Agent Skills](https://img.shields.io/badge/Claude-Agent%20Skills-da7756)

## Why it exists

Rankings and traffic are inputs. Leads and revenue are the output. A page that ranks well and converts nobody is a problem, not a win. These skills hold that line. They read the same data a serious growth practitioner reads, in the same order, and they refuse to recommend a fix without the evidence behind it.

The framing comes from my book, *CITED: The Growth Operating System for AI Search*. Search now splits across blue links and AI answers. This suite is built for both, and for the part that actually pays the bills: turning demand into qualified pipeline.

## The twelve modules

All twelve modules are written and usable. The suite covers the full search lifecycle plus AEO, GEO, SXO, E-E-A-T, CRO, and lead-tied reporting, with the CITED framework audit tying it to the book.

| Module | Status | What it does |
| --- | --- | --- |
| `cited-framework` | Ready | Audits a brand against the CITED framework, five layers (Citation Surface, Information Architecture, Technical Foundation, Evidence-Rich Extraction, Demand Capture), and runs the Citation Flywheel. |
| `growth-audit` | Ready | Revenue-weighted, full-funnel audit across Ahrefs, GSC, GA4, Clarity, CWV, and lead data. Ranks findings by business impact, not severity. |
| `technical-foundation` | Ready | Crawl, index, render, and Core Web Vitals from field data, with deploy-time drift checks so wins do not regress. Programmatic checks included. |
| `search-demand-map` | Ready | Keyword, intent, SERP-feature, and topic-cluster mapping scored by lead value and buying stage, not raw volume. |
| `content-engine` | Ready | Gap analysis against real competitors, E-E-A-T and citability, publishing sequence by time-to-rank, multimodal briefs, scored against pipeline. |
| `search-experience` | Ready | SXO. Reads the SERP backward to find page-type mismatch, derives the user stories behind a query, and scores the page per persona. |
| `conversion-cro` | Ready | Finds the friction between traffic and leads using GA4, Clarity, and CRM data, then prescribes specific UX, UI, and CRO fixes. |
| `ai-search-visibility` | Ready | Get cited in AI Overviews, AI Mode, ChatGPT, Perplexity, Gemini, and Copilot. Citation surfaces, llms.txt, entity signals, share of voice. |
| `structured-data-engine` | Ready | JSON-LD, entity and knowledge-graph markup, and rich-result eligibility, tied to the SERP features worth winning. |
| `authority-engine` | Ready | Backlink profile, anchor health, toxic-link triage, competitor link gap, and a prioritized digital-PR target list. |
| `competitive-intelligence` | Ready | Competitor SEO, content, and SERP ownership, plus share of voice across classic and AI search. |
| `growth-intelligence` | Ready | One reporting layer over Ahrefs, GSC, GA4, Clarity, and your CRM, tying rankings and traffic to leads and revenue. |

## How the suite fits together

The modules pass work to each other. A `growth-audit` produces a prioritized plan and hands the technical items to `technical-foundation`, the demand gaps to `search-demand-map`, the page friction to `conversion-cro`, and the tracking to `growth-intelligence`. You can run any one alone, or chain them into a full engagement.

## Speed to results

Search does not rank on a seven-day promise, and this suite will not pretend it does. What it does is find the fastest honest wins first and sequence the slow work behind them.

- Days to a few weeks: technical unblocks that free indexing, schema that wins a rich result, restructuring a page that already ranks so it earns a snippet or an AI citation, and refreshing a decaying page.
- Weeks: page-two pushes on commercial queries, comparison and alternatives pages where competition is weak, on-page and intent fixes.
- Weeks to months: new content authority, backlinks and earned media, entity recognition, and AI citation share.

Every module flags its quick wins and states realistic timeframes as ranges. Fast where fast is real, patient where it is not.

## Install

### Claude Code (plugin marketplace)

```bash
/plugin marketplace add avikbal-dm/growth-operating-system
/plugin install growth-os@avikbal-growth-os
```

### Claude Code or Desktop (manual)

```bash
git clone https://github.com/avikbal-dm/growth-operating-system.git
cp -r growth-operating-system/plugins/growth-os/skills/* ~/.claude/skills/
```

### Claude.ai

Zip the folder of the skill you want from `plugins/growth-os/skills/`, then upload it under **Settings > Capabilities > Skills**.

## A note on the data

These skills assume you have access to the accounts they read: Ahrefs, Search Console, GA4, Clarity, and a CRM or lead source. They describe the method. You bring the data and the judgment. Treat the projected outcomes as ranges, not promises, and validate against your own results.

## Author

Avik Bal is a B2B digital marketing practitioner specializing in web architecture, SEO, content strategy, and marketing analytics. He has helped enterprise software, fintech, and technology companies drive growth through scalable digital marketing programs. Avik is the author of *CITED: The Growth Operating System for AI Search*.

- LinkedIn: https://www.linkedin.com/in/avikbal/
- GitHub: https://github.com/avikbal-dm

## License

Released under the MIT License. See [LICENSE](LICENSE).

---
name: conversion-cro
description: >
  Diagnose and fix the gap between traffic and leads using real behavior data.
  Reads GA4 engagement and conversion paths, Microsoft Clarity heatmaps and
  session recordings, Core Web Vitals field data, and actual lead or CRM
  records, then finds the friction costing pipeline and prescribes specific UX,
  UI, and CRO fixes. Use when someone asks why a page gets traffic but no leads,
  wants a CRO audit, a UX or UI review tied to conversion, form or funnel
  analysis, landing page optimization, or help turning visitors into qualified
  leads. Every recommendation is grounded in observed behavior, not best-practice
  guesswork.
author: Avik Bal
---

# Conversion and CRO

## What this does

This skill finds where qualified visitors quit before becoming leads, and why. It works backward from the lead, through the form, the page, and the experience, using what users actually did rather than what a best-practice list assumes they do.

A higher conversion rate is not the goal on its own. More qualified leads is. A page can lift form fills with a weaker offer and produce worse pipeline. Judge against lead quality, not raw conversions.

## When to use it

Use it when a page or funnel has traffic but thin leads, when a redesign needs a conversion lens, or when sales complains about lead quality and the cause might be the page that captured them. Skip it for pages with no demand. Send those to `search-demand-map` first, because optimizing the conversion of a page nobody visits earns nothing.

## The data, and what each layer reveals

- **GA4**: engagement rate, key events, funnel exploration, and the page paths that precede a lead versus the ones that dead-end. This tells you where drop-off happens.
- **Microsoft Clarity**: the why behind the drop-off. Heatmaps show what users click and ignore. Recordings show hesitation, mis-clicks, and abandonment. Watch specifically for rage clicks, dead clicks, excessive scrolling, and quick-backs.
- **Core Web Vitals (field, p75)**: a slow LCP or a janky INP on a form page is a silent conversion leak. A form that lags on submit loses people who meant to convert.
- **Lead and CRM data**: which pages produce leads that sales actually wants. This separates a page that converts from a page that converts well.

Pair quantitative and qualitative on every finding. GA4 says where. Clarity says why. Neither alone is enough.

## Method

### 1. Define the conversion that matters

Name the real goal for this page or funnel. For B2B that is usually a demo request, a qualified contact, or a gated asset that feeds nurture. Map the steps a visitor takes to reach it.

### 2. Locate the leak with GA4

Build the path from entry to conversion and find the step with the steepest qualified drop-off. Separate intent first. A high exit on a top-of-funnel blog is normal. A high exit on a pricing page is a problem.

### 3. Explain the leak with Clarity

Pull recordings and heatmaps for the leaking step. Look for the specific friction: a CTA below the fold that no one reaches, a form field that triggers abandonment, a dead click on an element that looks interactive but is not, rage clicks signaling frustration, a layout shift that moves the button as they tap.

### 4. Check the experience tax

Read field CWV for the page. If INP or LCP sits in the poor band, the page is taxing every interaction. Note it as a conversion issue, not just a technical one, since that reframes the priority.

### 5. Audit the offer and the form

The form is where intent meets friction. Count the fields and challenge each one against lead quality. More fields can raise quality and lower volume, which is sometimes right for B2B and sometimes not. Decide with CRM data, not preference. Check the CTA wording, the value exchange, and whether the page answers the buyer's question before it asks for theirs.

### 6. Tie it back to lead quality

Before recommending a change that lifts volume, confirm it will not flood sales with weak leads. The win is qualified pipeline, so validate against CRM, not the conversion percentage alone.

## What you produce

For each finding: the leak, the GA4 evidence that located it, the Clarity evidence that explained it, the specific fix, and the expected effect on qualified leads as a range. Order by pipeline impact over effort. Where a test is warranted, propose it as an A/B with a clear hypothesis and the metric that decides it, not a vague "try this."

## Guardrails

- No fix without observed behavior behind it. Best practice is a hypothesis, not evidence.
- Separate what users did from why you think they did it. Recordings show behavior. The motive is your read.
- Watch for survivorship bias. The people who converted are not the ones you need to understand. Study the ones who left.
- A conversion lift that lowers lead quality is a loss. Always check the CRM side.

## Hands off to

`technical-foundation` when the friction is speed or stability, `content-engine` when the page fails to answer buyer intent, `structured-data-engine` when a richer SERP listing would pre-qualify the click, and `growth-intelligence` to confirm the change moved leads, not just the rate.

---

## About the author

Avik Bal is a B2B digital marketing practitioner specializing in web architecture, SEO, content strategy, and marketing analytics. He has helped enterprise software, fintech, and technology companies drive growth through scalable digital marketing programs. Avik is the author of *CITED: The Growth Operating System for AI Search*.

Part of the Growth Operating System. https://github.com/avikbal-dm/claude-seo-skills

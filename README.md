# AI proof-of-concepts for Innova

Two working AI tools built for [Innova](https://www.innova.it), the ductless heat-pump manufacturer, as part of an AI Growth Manager application. Both are static, self-contained, and run entirely in the browser - no build step, no backend, no keys.

**Live:** https://mattdevops.github.io/innova-ai-demos/

## The tools

### 1. Field Assist - `/field-assist`
A troubleshooting copilot for field technicians. A tech types a fault in plain language ("E4 in cold weather", "water dripping") and gets a step-by-step fix, a safe/caution/stop status, and the exact manual page it came from. Grounded in the real Innova/Ephoca 2.0 error codes (E1-E5, from the Installation & Maintenance Manual, Error Codes p.38).

### 2. DocSync - `/docsync`
A documentation consistency dashboard for a four-country manufacturer. When a spec changes, DocSync finds every manual, datasheet and compliance sheet that references it - in every language - flags what went stale, and drafts the edit. Solves the "old figure ships in a French datasheet" problem before it reaches a customer.

## What's real vs. illustrative

- **Real:** the product lines (2.0 HP DC Inverter, R290 monobloc, STONE), the 2.0 error codes and their descriptions, and the EU F-Gas / R290 regulatory context.
- **Illustrative:** the seeded document catalog and specific figures in DocSync are sample data to show the mechanism. Field Assist retrieves from a seeded slice of the manual so it runs with zero setup.
- In production, both connect to Innova's actual manuals and spec system, with a live model doing retrieval and drafting behind private infrastructure.

## Structure

```
index.html            landing page linking both tools
assets/base.css       shared design system (tokens, layout, components)
field-assist/         tool 1 (conversational)
docsync/              tool 2 (dashboard)
```

## Hosting

Static files, so it deploys anywhere with no configuration:

- **GitHub Pages:** Settings -> Pages -> deploy from `main`, root.
- **Vercel:** import the repo, framework preset "Other", no build command.

Built by Matthew Hasson.

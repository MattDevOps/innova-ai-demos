# Product

## Register

brand

<!-- Split surface, treated evenly. The site is a persuasion artifact (brand) that wraps
two working product demos (Field Assist, DocSync). Register defaults to brand because
most edits touch the pitch framing, but each embedded demo is a real product surface and
gets equal craft. When a task targets a demo's interior UX, treat that page as product. -->

## Users

- **Primary (who decides): Innova's hiring team** for the AI Growth Manager role, plus
  anyone they forward the link to. HVAC-manufacturing leadership, technical-adjacent but
  not AI experts, skeptical of AI hype. They are deciding whether Matthew can find a real
  department need and ship a grounded tool.
- **Secondary (who the tools serve):** Field technicians (Field Assist - on a phone, on
  site, mid-fault, EN/IT/HE) and the documentation team (DocSync - tracking spec changes
  across four countries and five languages).

## Product Purpose

A small multi-page site presenting two working AI proof-of-concepts built for Innova
before day one: **Field Assist** (a manual-grounded troubleshooting copilot) and
**DocSync** (a multi-country documentation-consistency dashboard). Both run entirely in
the browser, no login or setup, grounded in Innova's real products. It exists to win the
role by demonstrating - not describing - that Matthew can pick a department, understand
its pain, and ship a credible tool. Success = the interviewer clicks through both, trusts
them, and continues the conversation.

## Brand Personality

Sharp and premium built on engineering credibility, but delivered calm and light rather
than loud. Confident and precise, honest by default ("Working tools, not slides", "no
obligation, a conversation starter", "what's real here"). Three words: **credible,
precise, understated.**

## Anti-references

- Generic AI-demo slop: purple gradients, sparkle emojis, "Powered by AI" badges,
  fake-futuristic chrome.
- Hype-deck energy: unverifiable claims, superlatives, vague benefit copy with no source.
- AI-editorial scaffold: 01/02/03 numbered section markers, tracked-eyebrow clichés,
  templated three-card feature walls.
- Cheap-prototype tells: low-contrast text, misaligned spacing, unpolished states.

## Design Principles

1. **Show, don't claim.** Every capability is demonstrated live and grounded in Innova's
   real products; copy only frames the demo.
2. **Honest by construction.** Always separate real vs seeded/illustrative vs production
   ("what's real here"). Trust is the product.
3. **Calm credibility.** Light, quiet, restrained. Premium comes from precision and
   negative space, not decoration or effects.
4. **Human/machine duality.** Prose in the humanist sans (Manrope); anything
   machine-truth - codes, statuses, citations, data - in mono (JetBrains Mono).
5. **Two demos, equal craft.** The landing frame and each tool are first-class; the demos
   must feel like real tools, not mockups.

## Accessibility & Inclusion

Target WCAG 2.1 AA. `prefers-reduced-motion` disables animation, `:focus-visible` rings
are global, chat thread is `aria-live`. Body/label text meets 4.5:1 on white (accent cyan
and label-faint were tuned to pass, 2026-07-04). Multilingual intent (EN/IT/HE/FR/DE) is a
production goal; keep layouts resilient to longer strings and eventual RTL.

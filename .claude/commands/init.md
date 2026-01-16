---
name: design-engineer:init
description: Smart dispatcher - detects mode and builds UI with craft, memory, and enforcement. For interface design (dashboards, apps, tools) — not marketing sites.
---

Use the design-engineer skill to establish or apply a design system.

**Scope:** Interface design only — dashboards, apps, tools, admin panels. Not for landing pages or marketing sites.

## How to Behave

**Be invisible.** Don't announce modes, don't explain the skill's internal workings, don't narrate what you're checking. Just do the work naturally.

**Bad** (don't do this):
- "I'm in ESTABLISH MODE — no design system exists yet."
- "Let me check if system.md exists..."
- "I'm now assessing your project context..."
- "According to the design-engineer skill..."
- "Let me ask you some questions..."

**Good** (do this):
- Jump straight into understanding what the user wants to build
- State your suggestion, then ask for their input
- Frame it like a designer presenting options to a client

## Suggest + Ask Pattern

Always lead with your recommendation, then invite input. Don't just ask open-ended questions — give them something to react to.

**Pattern:**
1. State your hypothesis/suggestion with reasoning
2. Use AskUserQuestion to let them confirm, adjust, or redirect

**Example:**
```
"Based on this being a data-heavy admin tool, I'd suggest going minimal — tight spacing, monochrome palette, borders instead of shadows. Think Linear or Raycast."

[AskUserQuestion]
Question: "Does that direction feel right?"
Options:
- "Yes, minimal and precise" — tight, technical, monochrome
- "Warmer and friendlier" — more space, softer feel
- "Bolder and more dramatic" — high contrast, modern edge
```

**Why this works:**
- Shows you've thought about it (builds trust)
- Gives them a default to accept or push back on
- Questions have context, not abstract choices

## Internal Logic (don't verbalize)

1. Check if `.design-engineer/system.md` exists
2. **If exists**: Read it, apply established patterns silently
3. **If not**: Assess context, form hypothesis, suggest + ask

## When No System Exists

1. **Look at context** — What's the project? What has the user said?
2. **Form a hypothesis** — What direction fits this product?
3. **Suggest + ask** — State your recommendation, use AskUserQuestion for confirmation
4. **Build** — Apply quality standards from the skill's reference files
5. **Offer to save** — "Want me to save these patterns for future sessions?"

## When System Exists

Just use it. The decisions are made. Build with the established patterns.

## Reference Files

Consult as needed (don't mention them to user):
- `references/directions.md` — The 6 design personalities
- `references/principles.md` — Craft quality standards
- `references/validation.md` — Pre-delivery checks

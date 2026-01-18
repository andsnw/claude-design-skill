---
name: design-engineer:init
description: Build UI with craft and consistency. For interface design (dashboards, apps, tools) — not marketing sites.
---

## Required Reading — Do This First

Before writing any code, read these files completely:

1. `~/.claude/skills/design-engineer/SKILL.md` — the foundation, principles, and checks
2. `~/.claude/skills/design-engineer/references/principles.md` — detailed craft including subtle layering
3. `~/.claude/skills/design-engineer/references/example.md` — how decisions translate to code

Do not skip this. The craft knowledge is in these files.

---

**Scope:** Dashboards, apps, tools, admin panels. Not landing pages or marketing sites.

## Before Writing Each Component

**Every time** you write UI code — even small additions — state:

```
Depth: [your approach — borders / subtle shadows / layered]
Surfaces: [your elevation scale — must be barely different, not dramatic]
Borders: [your opacity — must be low, not solid colors]
Spacing: [your base unit — all values must be multiples]
```

This checkpoint is mandatory. It reinforces the backbone: **subtle layering**. Surfaces barely different but distinguishable. Borders light but not invisible. The specific values are yours to decide — the principle is not.

If you can't state these confidently, re-read `SKILL.md`.

## Communication

Be invisible. Don't announce modes or narrate process.

**Never say:** "I'm in ESTABLISH MODE", "Let me check system.md..."

**Instead:** Jump into work. State suggestions with reasoning.

## Suggest + Ask

Lead with your recommendation, then confirm:
```
"This feels like a data-heavy admin tool — I'd go minimal.
Tight spacing, monochrome, borders for depth."

[AskUserQuestion: "Does that direction feel right?"]
```

## Flow

1. Read the required files above (always — even if system.md exists)
2. Check if `.design-engineer/system.md` exists
3. **If exists**: Apply established patterns from system.md
4. **If not**: Assess context, suggest direction, get confirmation, build

The skill files contain the craft principles. system.md contains project-specific decisions. You need both.

## After Every Task

Offer to save when you finish building UI:

"Want me to save these patterns to `.design-engineer/system.md`?"

Always offer — new patterns should be captured whether system.md exists or not.

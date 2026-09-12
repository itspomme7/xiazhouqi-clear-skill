# Xiazhouqi Clear Skill

> **Xiazhouqi Clear｜下周七·清透** — a calm, information-first web design skill for dense personal utility pages.

[简体中文](./README.zh-CN.md) · [Full specification](./SKILL.md) · [Changelog](./CHANGELOG.md)

Part of the **[Xiazhouqi](https://xiazhouqi7.com)** design system.

## What it is

Xiazhouqi Clear is built for pages that carry a lot of real information but still need to feel clean, restrained, readable, and reliable on mobile.

It keeps the restraint of Apple-like interface design without copying Apple. Its own hierarchy comes from structure, typography, shadow, spacing, and restrained semantic color.

> **Structure creates order · Weight creates emphasis · Shadow creates depth · Color creates classification**

## Best for

- email and account archives
- Apple ID / region account management
- bank-card and finance pages
- spending plans and personal dashboards
- private archive entrances
- download centers and utility pages
- long-lived single-file HTML tools

## Core rules

- Content first; decoration second
- Group information before styling it
- Clear is not pure black, white, and gray
- Use low-saturation color only when it carries meaning
- Keep the page shell neutral; never tint the body, every card, every tag, and every control with the same accent
- Core / Normal / Quiet content must not share the same visual weight
- Utility controls stay small and quiet, but interaction must remain reliable
- Mobile must have zero horizontal overflow
- Password, enter, switch, and primary-content visibility must not rely on fragile JavaScript alone when a resilient fallback is possible
- Never invent explanatory copy just to make a layout look designed
- Preserve source data unless the user explicitly changes it

## Current release

**v1.2.0 — 2026-09-12**

This release promotes the approved email and spending-plan pages to canonical references, makes neutral dominance a hard rule, prohibits page-wide single-accent tinting, and adds patterns for daily-task, annual-goal, and history views.

## Repository structure

```text
.
├─ README.md
├─ README.zh-CN.md
├─ SKILL.md
├─ CHANGELOG.md
├─ VERSION
├─ tokens.css
├─ reference.html
├─ LICENSE
├─ .gitignore
├─ references/
│  ├─ canonical-visual-patterns.md
│  ├─ hierarchy-and-color.md
│  ├─ content-patterns.md
│  ├─ mobile-and-compatibility.md
│  ├─ copy-and-content.md
│  └─ maintenance-and-checklist.md
└─ examples/
   ├─ README.md
   └─ clear-information-cards.html
```

## Trigger phrases

`xiazhouqi-clear` · `Xiazhouqi Clear` · `下周七·清透` · `清透风格` · `苹果感但不要照抄苹果` · `信息多但要耐看`

## Xiazhouqi system

- **Clear** — restrained, information-first interface design
- **[Warm](https://github.com/xiazhouqi7/xiazhouqi-warm-skill)** — soft, warm and personal visual design
- **[Photography](https://github.com/xiazhouqi7/xiazhouqi-photography-skill)** — photography, grading and visual storytelling

## License

MIT

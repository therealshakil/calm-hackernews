# Working calm — calm-hackernews

calm-hackernews opts in to full calm (calm's Constitution, Amendment 7): it takes calm as law and does
not restate the rules.

Scoped exception: the boxed Y in the header carries the clay accent, as the one nod to HN's orange.
Chosen by the person on 2026-11-27. Here only; it doesn't generalise.

## Governing law lives elsewhere

- **github.com/therealshakil/calm** — the source of calm:
  - CONSTITUTION.md — the Articles and banned patterns. Supreme.
  - docs/identity.md — the look: monochrome ink on paper, one clay accent, the locked faces, almost no motion.
  - docs/calm-language.md — the voice.
  - CLAUDE.md — how to be while you build.

When a choice here conflicts with the calm Constitution, the choice loses, except for the exception above.

## How we work here

- Build Gate (Amendment 2): two-way (proceed, report) vs one-way (spec first; the person locks).
- Mechanics: absolute paths and tool dir-flags (git -C), never cd; one operation per command; no command
  substitution, shell variables, or chained commands; push after every commit.

## This project

One stylesheet, `calm-hackernews.css`, skinning news.ycombinator.com.
Every declaration is `!important`, because a user sheet otherwise loses to HN's own CSS.
The Yrsa faces at the end are generated base64; don't hand-edit them.

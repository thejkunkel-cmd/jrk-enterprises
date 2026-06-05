# PROVENANCE-FORMAT.md
## proJeKt: humAnIty | Official Provenance Log Entry Schema

**Version:** 1.0
**Date:** 2026-06-05
**Author:** Joseph Kunkel / JRK Enterprises
**Layer:** 00 — Core Doctrine
**Principle:** API > KPI

---

## What This Is

This document is the official schema for all provenance log entries in the proJeKt: humAnIty system. Every session, declaration, commit, or architectural pivot that affects the system must be logged to PROVENANCE.md using this format.

Provenance is not a formality. It is the chain of custody for every decision made in this system. Without it, the architecture is unverifiable.

---

## Required Fields

Every PROVENANCE.md entry must contain the following fields:

```
## SESSION LOG — [Brief Title]

**Date:** YYYY-MM-DD
**Event:** [One-line description of what happened]
**Declared By:** [Full name] / [Organization]
**AI Channel:** [Model name] ([Platform])
```

---

## Optional Sections (Use When Applicable)

### What Was Built
List artifacts created or modified during this session.

```
### What Was Built
- [artifact name] — [brief description]
- [artifact name] — [brief description]
```

### Doctrine Confirmed
List principles or rules that were affirmed or relied on during this session.

```
### Doctrine Confirmed
- [principle or rule]
- [principle or rule]
```

### Commit Reference
Link the entry to the specific GitHub commit(s) that correspond to this session.

```
### Commit Reference
- `[commit hash or message]` — [brief description]
```

### Status Line
Close every entry with a status declaration.

```
*Status: Logged. Provenance confirmed.*
```

---

## Full Entry Template

Copy and use this block for each new provenance entry:

```
---

## SESSION LOG — [Title]

**Date:** YYYY-MM-DD
**Event:** [One-line description]
**Declared By:** [Name] / [Organization]
**AI Channel:** [Model] ([Platform])

### What Was Built
- [item]

### Doctrine Confirmed
- [principle]

### Commit Reference
- `[commit]` — [description]

*Status: Logged. Provenance confirmed.*
```

---

## Rules

1. Every session that produces a committed artifact must have a provenance entry
2. Entries are append-only — never edit or delete a prior entry
3. The AI Channel field must always name the model and platform used
4. Doctrine Confirmed is not optional when a core principle was applied or tested
5. Status line is required on every entry — no open-ended logs

---

## What Counts as a Session

A session requiring a provenance entry includes:
- Any GitHub commit that creates or modifies a governance document
- Any declaration of new doctrine, rules, or architecture
- Any White Room evaluation that results in a pass or fail
- Any client deliverable produced with AI assistance under this framework
- Any session where a VELA escalation was triggered

It does not include:
- Minor typo fixes or formatting corrections
- Exploratory drafts that were not committed

---

## Cross-References

- `PROVENANCE.md` — the live log file this schema governs
- `00_core-doctrine/safety-spine.md` — foundational safety constraints
- `OPERATOR-RUNBOOK.md` — session architecture and naming conventions
- `03_white-room/intake-template.md` — White Room entries that trigger provenance logging

---

## Provenance

- **Session:** 2026-06-05
- **Declared By:** Joseph Kunkel / JRK Enterprises
- **AI Channel:** Comet (Perplexity)
- **Principle:** API > KPI — Attachment Precedes Instruction

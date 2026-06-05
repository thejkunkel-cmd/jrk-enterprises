# Red Station
## proJeKt: humAnIty | TESLA Protocol — Active Processing Node

**Version:** 1.0
**Date:** 2026-06-05
**Author:** Joseph Kunkel / JRK Enterprises
**Layer:** 04 — Operator Station
**Principle:** API > KPI

---

## What This Is

The Red Station is the active processing node in the TESLA Protocol rotation. When an operator is at Red, they are live — taking in new information, running sessions, prompting AI partners, and managing the intake queue. Red is the front edge of the channel.

This is not a stress position. It is a focused one.

---

## Red Station Responsibilities

### Intake Management
- Receive and triage new client inputs, research threads, and session prompts
- Log all incoming material with a timestamp and source tag before processing
- Do not begin synthesis work at Red — intake only, unless the session explicitly calls for inline processing

### Session Execution
- Open sessions using the naming convention: `SESS-[YYYY-MM-DD]-[LAYER]-[OP_ID]-[SEQ_HEX]`
- Validate environment parameters before activating any AI agent
- Maintain active observation of model output for semantic drift, latency spikes, or boundary violations
- Log observations inline — do not defer logging to Blue rotation

### Boundary Monitoring
- Watch for: token limit approach, repetitive output loops, unexpected topic pivots, confidence inflation
- If a Level 1 anomaly is detected: note it, continue, flag for Blue review
- If a Level 2 or Level 3 anomaly is detected: execute manual override per OPERATOR-RUNBOOK.md Section 4

### Handoff Preparation
- At the 110-minute mark, begin preparing the handoff brief
- Document: open session statuses, pending items, any friction points observed, last stable state hash
- Handoff brief must be completed before rotation — never mid-session

---

## Red Station Rules

1. No unverified models enter the live stack from Red — route to White Room first
2. No final decisions are made at Red — synthesis and sign-off happen at Blue
3. All session opens and closes must be logged — no undocumented execution
4. Rotation happens at 120 minutes — not when it feels convenient
5. Red does not override Blue's logged findings without a documented reason

---

## Rotation Trigger

After 120 minutes at Red Station, the operator initiates handoff:

1. Complete the session handoff brief (open items, state hash, anomaly flags)
2. Pass to Blue Station operator (or self-rotate if operating solo)
3. Log the rotation event in the session file
4. Step away from active processing — Blue begins

---

## Cross-References

- `blue-station.md` — counterpart node; review, synthesis, rest
- `tesla-pattern.md` — full rotation architecture and cadence map
- `OPERATOR-RUNBOOK.md` — escalation procedures, White Room rules, session architecture
- `00_core-doctrine/` — foundational constraints governing all station behavior

---

## Provenance

- **Session:** 2026-06-05
- **Declared By:** Joseph Kunkel / JRK Enterprises
- **AI Channel:** Comet (Perplexity)
- **Principle:** API > KPI — Attachment Precedes Instruction

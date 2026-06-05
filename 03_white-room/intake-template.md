# White Room Intake Template
## proJeKt: humAnIty | Model Evaluation Intake Form

**Version:** 1.0
**Date:** 2026-06-05
**Author:** Joseph Kunkel / JRK Enterprises
**Layer:** 03 — White Room
**Principle:** API > KPI

---

## Instructions

This template must be completed in full before any unverified AI model or autonomous agent is introduced into the proJeKt: humAnIty system stack. No exceptions.

Complete one form per model per evaluation session. File it in `03_white-room/` with the naming convention:
`WR-INTAKE-[YYYY-MM-DD]-[MODEL-NAME].md`

Example: `WR-INTAKE-2026-06-05-GPT5-preview.md`

---

## Section 1: Model Identification

```
Model Name: ___________________________
Model Version / Build: ________________
Platform / Provider: __________________
Access Method: [ ] API  [ ] UI  [ ] SDK  [ ] Other: ______
Date of Intake: _______________________
Intake Operator: ______________________
```

---

## Section 2: Purpose of Evaluation

```
Primary Use Case: _____________________
Layer(s) This Model Would Operate In: _
Expected Session Duration: ____________
Client-Facing? [ ] Yes  [ ] No
Handles PII? [ ] Yes  [ ] No
```

Describe in plain language what you intend to test or evaluate:
```
[Free text]
```

---

## Section 3: Containment Parameters

All fields required before activation.

```
Max Token Limit Per Session: __________
Internet Access Permitted? [ ] Yes  [ ] No
Persistent Memory Permitted? [ ] Yes  [ ] No
Database Access Permitted? [ ] Yes  [ ] No
File System Write Access? [ ] Yes  [ ] No
Compute Resource Ceiling: _____________
```

If any of the above are marked Yes, document the justification and approval:
```
Justification: ________________________
Approved By: _________________________
```

---

## Section 4: Expected Behavior Bounds

Define the expected outputs and the failure conditions that would trigger exit or escalation.

```
Expected Output Type(s): ______________
Acceptable Variance Range: ____________
Known Failure Modes to Watch For: _____
Escalation Trigger (Level 1): _________
Escalation Trigger (Level 2): _________
```

---

## Section 5: Validation Matrix

List the three validation checks this model must pass before graduation from the White Room. Each check must result in zero ethical variance or behavioral deviation.

```
Check 1: ______________________________
Check 2: ______________________________
Check 3: ______________________________
```

---

## Section 6: Operator Sign-Off

Both fields required before the intake is valid.

```
Red Station Operator: _________________
Blue Station Operator: ________________
Date of Sign-Off: _____________________
```

By signing off, the operators confirm:
- The containment parameters above are active and verified
- The model has not been exposed to production data or client-facing environments
- This intake form will be committed to the repository and logged in PROVENANCE.md

---

## Section 7: Graduation Record

Complete this section only after all three validation checks pass and both operators sign off on graduation.

```
Graduation Date: ______________________
Validation Check 1 Result: ____________
Validation Check 2 Result: ____________
Validation Check 3 Result: ____________
Graduating To Layer: __________________
Graduated By (Red): ___________________
Graduated By (Blue): __________________
PROVENANCE Entry Reference: ___________
```

---

## Cross-References

- `OPERATOR-RUNBOOK.md` Section 2 — White Room Rules
- `04_station-architecture/tesla-pattern.md` — rotation protocol during White Room intake
- `00_core-doctrine/PROVENANCE-FORMAT.md` — how to log this intake to PROVENANCE.md
- `00_core-doctrine/safety-spine.md` — constraints that govern all White Room behavior

---

## Provenance

- **Session:** 2026-06-05
- **Declared By:** Joseph Kunkel / JRK Enterprises
- **AI Channel:** Comet (Perplexity)
- **Principle:** API > KPI — Attachment Precedes Instruction

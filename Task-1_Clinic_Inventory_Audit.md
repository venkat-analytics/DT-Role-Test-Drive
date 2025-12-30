# Task 1: Clinic Inventory Daily Micro-Audit

## Objective
Detect small, frequent inventory and billing errors early in a clinic pharmacy
where medicines are manually entered, without increasing doctor involvement.

---

## Daily Checklist (20–30 mins)

### 1. High-Risk Medicine Focus
Criteria used:
- High sales volume
- Similar or confusing names
- Frequent prescriptions

| Medicine | Reason |
|--------|--------|
| Dolo 650 | High volume + name variations |
| Azithromycin 500 | Abbreviations commonly used |
| Pantoprazole 40 | Frequently prescribed |

---

### 2. Name-Variation Check (10 mins/day)
- Filter sales register for high-risk medicines
- Group entered variants under standard master names

| Variants | Master |
|--------|--------|
| Dolo / Dolo kind | Dolo 650 |
| Azithro / Azithromycin | Azithromycin 500 |

Action:
- Add new variants to mapping
- Inform billing staff

---

### 3. Usage Reasonableness Check (5 mins/day)

Expected Closing = Opening + Purchases − Sales

| Medicine | Expected | Actual | Action |
|--------|---------|--------|--------|
| Dolo 650 | 1,460 | 1,440 | Review sales entries |

Rule:
- Difference beyond ±2% is flagged

---

### 4. Random Bill Spot Checks (5–10 mins/day)
- Randomly review 3–5 bills
- Verify medicine name and quantity reasonableness
- Log and correct errors

---

## Weekly Control (15 mins)

### Error Pattern Tracking
- Maintain simple error log
- Same error ≥3 times → retraining
- Multiple medicines affected → SOP clarification

---

## Doctor Escalation
Doctor involved only if:
- Financial impact is material
- Errors persist despite correction
- Treatment availability is affected

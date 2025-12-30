# Task 1: Clinic Inventory Daily Micro-Audit

## Objective
Detect small, frequent inventory and billing errors early in a clinic pharmacy
where medicines are manually entered, without increasing doctor involvement
or disrupting OPD and billing rush hours.

---

## Daily Checklist (20–30 mins)

This checklist is designed to run during low-patient-load windows so that
inventory discipline improves without slowing down front-desk or billing work.

---

### 1. High-Risk Medicine Focus
Instead of checking all medicines, the audit focuses only on medicines where
errors are most likely to occur in day-to-day clinic operations.

Criteria used:
- High sales volume
- Similar or confusing medicine names
- Frequent prescriptions by the doctor

| Medicine | Reason |
|--------|--------|
| Dolo 650 | High volume + name variations during manual entry |
| Azithromycin 500 | Abbreviations commonly used by staff |
| Pantoprazole 40 | Frequently prescribed across OPD visits |

---

### 2. Name-Variation Check (10 mins/day)
Manual typing leads to inconsistent medicine names, especially during peak OPD
hours. This step catches those variations early.

What I do:
- Filter the sales register for high-risk medicines
- Group entered variants under standard master names

| Variants | Master |
|--------|--------|
| Dolo / Dolo kind | Dolo 650 |
| Azithro / Azithromycin | Azithromycin 500 |

Action:
- Add any new variant to the mapping list
- Inform billing staff to use the standard master name going forward

---

### 3. Usage Reasonableness Check (5 mins/day)
For each high-risk medicine, I check whether daily sales and stock movement
look reasonable instead of doing full reconciliation.

Expected Closing = Opening + Purchases − Sales

| Medicine | Expected | Actual | Action |
|--------|---------|--------|--------|
| Dolo 650 | 1,460 | 1,440 | Review sales entries |

Rule:
- Any difference beyond ±2% is flagged and reviewed the same day

This prevents small daily mistakes from becoming large month-end surprises.

---

### 4. Random Bill Spot Checks (5–10 mins/day)
To improve billing discipline without creating fear or fixed routines,
random bill checks are used.

What I do:
- Randomly review 3–5 bills containing high-risk medicines
- Verify medicine name accuracy and quantity reasonableness

Random checks are preferred because staff tend to be more careful when checks
are unpredictable, especially during busy OPD hours.

Errors are logged and corrected without penalties.

---

## Weekly Control (15 mins)

### Error Pattern Tracking
A simple error log is maintained to identify repeated issues.

- Same error occurring 3 or more times → targeted retraining
- Errors across multiple medicines → SOP clarification or update

This shifts the focus from daily corrections to root-cause improvement.

---

## Doctor Escalation
Doctor involvement is strictly limited and triggered only when necessary.

Doctor is involved only if:
- Financial impact is material
- Errors persist despite correction
- Inventory mismatch affects treatment availability

All routine checks and corrections are handled without disturbing the doctor.


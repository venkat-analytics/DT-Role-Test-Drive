# Task 2: Patient Care & Communication Control System

## Objective
Reduce doctor interruptions and WhatsApp chaos while ensuring patients receive
timely, consistent care communication using existing clinic systems.

The system is designed to absorb routine communication and surface only
exceptions that require medical judgment.

---

## 1. Message Classification (One-Time Setup)

Patient messages are first classified based on whether doctor input is required.
This prevents the doctor from being involved in routine, repeatable communication.

| Message Type | Example | Doctor Input Needed |
|-------------|--------|-------------------|
| Follow-up Reminder | “Please visit on Aug 5” | No |
| Post-Procedure Care | “Mild swelling is normal” | No |
| Side-Effect Advisory | “Nausea may occur” | No |
| Custom Instruction | “Avoid sun exposure for 7 days” | Yes |
| Patient Question | “Is itching normal?” | Yes |

This classification ensures doctor attention is used only where judgment is required.

Time: 20 minutes (one-time)

---

## 2. Care Control Sheet (Daily Working Sheet)

All patient communication is tracked in a single Google Sheet named `Care_Control`.
This sheet acts as the single source of truth for follow-ups and messages.

| Patient | Phone | Visit Type | Message Type | Message Text | Doctor Approval | Status |
|-------|------|-----------|-------------|--------------|----------------|-------|
| Ramesh K | 9XXXX | OPD | Follow-up | Auto-filled | Not Required | Pending |
| Sita P | 9XXXX | Procedure | Post-Procedure | Auto-filled | Not Required | Pending |
| Arjun M | 9XXXX | OPD | Custom | Blank | Required | Waiting |

Routine messages are auto-filled.
Only messages requiring judgment remain blank.

---

## 3. Doctor Review Window (Every 3–4 Hours)

Instead of responding continuously, doctor input is batched.

What happens:
- Filter the sheet where:
  - Doctor Approval = Required
  - Status = Waiting
- Sit with the doctor for a focused 10-minute window
- Doctor approves or dictates responses
- Staff updates the sheet immediately

Doctor never:
- Opens WhatsApp
- Types messages
- Tracks follow-ups mentally

This minimizes context switching during OPD hours.

---

## 4. Patient Question Handling (Google Form Flow)

To avoid ad-hoc WhatsApp questions, patients submit queries via a Google Form.

Form fields:
- Name
- Phone number
- Question
- Urgency (Routine / Urgent)

Responses populate a sheet called `Patient_Questions`.

Questions are reviewed in batches every 3 hours and answered in one short
doctor interaction instead of multiple interruptions.

---

## 5. Message Dispatch Rules

Messages are sent only when all conditions are satisfied:
- Message text is filled
- Status = Pending
- Doctor Approval = Not Required or Approved

Status flow:
Pending → Sent → Closed

This prevents accidental, incomplete, or unapproved communication.

---

## 6. Daily Closing Check (5 mins)

Before clinic closes:
- Filter messages with Status = Pending
- Ensure no urgent or important follow-ups are missed
- Reschedule or flag items if needed

This acts as a final safety net for patient care.

---

## Why This System Works
- Routine communication is automated
- Doctor time is protected and structured
- Human judgment is used only for exceptions
- Clinic staff can run the system daily without stress


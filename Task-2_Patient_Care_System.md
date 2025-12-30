# Task 2: Patient Care & Communication Control System

## Objective
Reduce doctor interruptions and WhatsApp chaos while ensuring timely,
consistent patient communication.

---

## 1. Message Classification
| Message Type | Doctor Input Needed |
|------------|-------------------|
| Follow-up reminders | No |
| Post-procedure care | No |
| Side-effect advisory | No |
| Custom instructions | Yes |
| Patient questions | Yes |

---

## 2. Care Control Sheet
Single Google Sheet: Care_Control

| Patient | Message Type | Doctor Approval | Status |
|-------|-------------|----------------|--------|
| Ramesh | Follow-up | Not Required | Pending |
| Arjun | Custom | Required | Waiting |

---

## 3. Doctor Review Window
- Every 3–4 hours
- Filter: Approval = Required & Status = Waiting
- 10-minute batch review
- Staff records approved messages

Doctor never types or opens WhatsApp.

---

## 4. Patient Questions (Google Form)
- Patients submit questions via form
- Questions batched every 3 hours
- Answers recorded and sent together

---

## 5. Message Dispatch Rules
Messages sent only when:
- Message text is filled
- Status = Pending
- Approval = Not Required or Approved

Flow:
Pending → Sent → Closed

---

## 6. Daily Closing Check (5 mins)
- Review pending messages
- Ensure no critical follow-ups are missed

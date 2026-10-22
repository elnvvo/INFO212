# Ekte Mat Online – INFO212 project

Student project for INFO212 (Lab 7). The aim is to replace Ekte Mat AS's e-mail-, phone- and Excel-based ordering with an online ordering and event-booking system.

> **All data in this repository is synthetic.** Ekte Mat AS, its staff, customers (e.g. Fjordtek AS), orders and amounts are fictional and were created for INFO212 Lab 7.

## The case

Ekte Mat is a small catering company in Bergen that serves authentic, seasonal food to corporate customers (weekly lunches, meetings), private parties and weddings.

Draft vision (v0.3):

> For Bergen companies and families who want authentic, seasonal food for their events, Ekte Mat Online is an ordering and event-booking service that lets customers see menus, prices and food origin, book and change orders any time, and pay the way that suits them. Unlike ordering by e-mail and phone, it gives the kitchen one reliable overview of every order and allergy.

### Key facts and constraints

- **Budget:** 450 000 NOK for the first version, including 12 months of hosting. Running costs under 3 000 NOK/month.
- **Deadline:** go-live 1 March 2027 (hard). Wedding season starts in May 2027.
- **Team:** 3 student developers, 2-week sprints. Product owner Ingrid Solheim, available Tuesdays 09–10.
- **Integrations:** Fiken (accounting, REST API, EHF invoices), Vipps (private customers), Google Workspace (e-mail/calendar).
- **Data protection:** data must stay in the EU/EEA. Allergy information can be health data (GDPR art. 9), so store it per guest group. Keep bookkeeping data for 5 years. Support access and deletion requests.
- **UI:** Norwegian and English.
- **Kitchen capacity:** about 400 covers/day, or about 250 if there is a served wedding dinner that day.

### Points where stakeholders disagree

- **Deposits:** Ingrid wants a 30 % deposit on every booking. Sunniva and Fjordtek say corporate customers won't prepay and need one monthly EHF invoice. A deposit makes sense for weddings.
- **Build or buy:** the team hasn't decided whether to build its own system or configure an off-the-shelf catering SaaS.

## Files in this folder

### Stakeholder interviews

| File | Contents |
|---|---|
| `interview_Ingrid_owner.txt` | Owner Ingrid Solheim: lost inquiries, self-service booking, 30 % deposit, Vipps/Fiken, food origin, budget and deadline. |
| `interview_Sunniva_event_coordinator.txt` | Event coordinator Sunniva Berg: current workflow, reply times, capacity calendar, guest-number reminders, allergies per guest group. |
| `interview_Mateo_head_chef.txt` | Head chef Mateo Rinaldi: kitchen tablet with PIN login, seasonal menu editing, supplier/origin data, prep lists, offline mode, performance. |
| `interview_Fjordtek_customer.txt` | Corporate customer Henrik Aas (Fjordtek AS): company login, standing orders, approval limit, monthly EHF invoice with cost centres, EU/EEA data storage. |
| `Kopi av interview Sunniva (2).txt` | Exact duplicate of the Sunniva interview. Can be deleted. |

### Meetings, process and context

| File | Contents |
|---|---|
| `notes meeting 12 aug FINAL.txt` | Kick-off meeting: goals, integrations, customer groups, timeline, action items, open build-or-buy question. |
| `asis_order_process.md` | Current ("as-is") order process in 12 steps, from first customer contact to monthly reconciliation. |
| `current_IT_landscape.txt` | Current tools (Wix, Google Workspace, Excel, Fiken, Vipps) and constraints. |
| `budget and constraints.txt` | Budget, running-cost target, deadlines and team setup. |
| `GDPR note from consultant.txt` | Data-protection advice: health data, retention periods, access/deletion rights, data processing agreements. |
| `vision_draft_v0.3.docx` | Draft product vision statement. |

### Data exports

| File | Contents |
|---|---|
| `orders_2024_2025_export.xlsx` | Order history export. Sheet `Bestillinger` has about 820 orders (order/event date, customer type, channel, menu package, guests, prices, dietary notes, delivery, status). Sheet `README` explains the columns. |
| `customer_emails_export.csv` | Sample of incoming customer e-mails (Norwegian and English): booking requests, allergy questions, guest changes, invoice issues. |
| `lunch menu autumn.txt` | Draft autumn lunch menu with prices and allergens to label. |

### Other

| File | Contents |
|---|---|
| `competitor links.txt` | Competitor websites for benchmarking. |
| `logo ideas.txt` | Logo brainstorm. Not relevant to system development. |
| `untitled.txt` | Personal to-do notes (sprint 0: Git repo, task board, Definition of Done). |

## Running the application

There is no application code yet. When there is, this section will explain how to install and run it. Dependencies will be listed in `requirements.txt`, which is currently a placeholder.

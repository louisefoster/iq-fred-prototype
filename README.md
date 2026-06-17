# IQ Fred Prototype

An interactive prototype built for **IQ Accelerator Day — 23rd June 2026**, a focused session with sellers to bring IQ to life.

---

## Purpose

This prototype visualises what IQ means in practice — not how it works, but what it empowers a customer to do. It is **future state**: the products and workflows shown need to power up to fully enable it, but the experience demonstrates the destination.

The audience is sellers who are not aligned to standard ways of working. The goal is to make IQ tangible and compelling in under 30 minutes.

---

## The Story — Fred Ellison

Fred is an **Operations Director at a logistics company**. He has purchased the full IQ suite:

- Time & Attendance (inc. HR & AR)
- Payroll
- Planning & Tracking
- Financials
- Source-to-Contract (S2C)
- Purchasing
- Governance & Risk

Fred also works with **third-party systems**:
- **Qargo** — Transport Management System (TMS)
- **Eploy** — Recruitment platform

The prototype shows **Fred's Tuesday morning** — a session that used to take 3 hours of calls and spreadsheets, resolved in under 6 minutes through IQ.

---

## The Walk-Through

The prototype is a single interactive session. The presenter clicks through Fred's morning in order.

### 1. IQ Home — Fred's Intelligent Briefing
IQ proactively opens Fred's day with three action items surfaced from across his connected systems:

- **Driver hours risk** — 4 drivers near their Working Time Directive (WTD) limit, with 3 Qargo deliveries still assigned (T&A + Qargo)
- **Payroll closes Friday** — 14 timesheets unconfirmed, 3 new starters not yet validated (Payroll + T&A)
- **AI Compliance flag** — a complaint pattern detected on the East Midlands route (G&R + AI Module)

Fred didn't ask for any of this. IQ surfaced it.

---

### 2. Driver Hours Risk → Resolve
Fred taps the Driver hours card. IQ pulls live T&A data and cross-references the Qargo delivery schedule, showing which drivers are at risk, which routes are affected, and how many stops remain.

**IQ suggests:** Reallocate 5 stops to J. Chen and M. Okoro (available capacity identified automatically).

Fred taps **Reassign & log decision** — the reallocation is logged simultaneously in T&A and G&R, and the Qargo schedule is updated. One action, three systems.

---

### 3. Finance Query — Agentic Moment
Fred types (or uses a quick prompt chip): *"How much are we spending on subcontractors vs plan this quarter?"*

IQ pulls from Financials, Purchasing orders, and S2C contract thresholds — returning a chart, three key stats, and a recommendation.

**IQ surfaces:** Subcontractor spend is 34% above plan (£198k vs £148k). Two S2C agreements allow renegotiation before August.

Fred taps **Draft commercial summary** — IQ stages the document for procurement review.

The sell: no BI team, no waiting. The answer is in the flow of work.

---

### 4. Recruit-to-Pay Pipeline — Third-Party Integration
Fred uses the quick prompt: *"Show driver pipeline from Eploy."*

IQ shows the full end-to-end chain: 3 live roles in Eploy → Offer & Contract (1 pending) → HR Onboarding → T&A from Day 1 → First Payslip.

**IQ explains:** Once the offer is signed in Eploy, every subsequent step triggers automatically — no manual handoff between systems.

The sell: a new driver hired through a third-party system flows seamlessly into the full OA stack.

---

### 5. AI Compliance — Pattern Detection
Fred taps the AI Compliance card. The AI Module has identified a pattern across 6 complaints — same depot, same 72-hour window, all delivery-window breaches.

**IQ root cause:** A Qargo scheduling conflict at the EM depot has assigned overlapping time windows between 13:00–15:30. Drivers cannot physically complete all stops.

**IQ suggests:** Raise a reportable incident in G&R (auto-populated) and fix the Tuesday Qargo schedule.

Fred taps **Raise incident & fix schedule** — both actions complete simultaneously.

The sell: IQ found the thing Fred didn't know to look for — before it became a formal incident.

---

## Key Design Principles

- **Proactive, not reactive** — IQ opens Fred's day without him asking
- **In the flow of work** — every action resolves across multiple systems from a single decision
- **Third-party aware** — Qargo and Eploy are native in the IQ experience, not separate logins
- **One thread** — the entire session is a single conversation surface, not a dashboard of charts
- **Action-first** — every insight has a primary action button; Fred is never left staring at data

---

## Running Locally

```bash
npm start
```

Opens on `localhost:3000`. No build step — it is a single self-contained HTML file.

---

## Deployment

The prototype is hosted separately from this repo. To deploy manually to any static host, serve `index.html` — no server or build process required.

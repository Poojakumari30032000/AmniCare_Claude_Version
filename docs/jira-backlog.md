# AmniCare Jira Backlog

Backlog created in Jira project **KAN** (`AmniCare_Claude_Version`) at
https://poojakumarismartdata.atlassian.net/browse/KAN-1

Derived from two source documents:

- `SCOPE_OF_WORK.docx` — solution, modules, user roles, functional requirements (N/A/S/C/B/O IDs), technology stack
- `Amnicare_Milestone_details.xlsx` — Milestone sheet (M1–M5, sprints 1–13), Tech Stack sheet, Feature listing sheet

**Totals:** 6 epics, 68 child issues (56 stories, 12 tasks).

Every issue description carries: milestone, sprint, SOW requirement ID, component,
delivery pod, a user story or objective, acceptance criteria, and a source reference
back to the originating document section.

## Epics

| Key | Epic | Milestone | Sprints | Weeks |
|---|---|---|---|---|
| KAN-1 | Core Multi-Tenancy, Security & Access Control | M1 | 1–2 | 1–4 |
| KAN-2 | EHR Lite: Client, Caregiver, Care Plan & Scheduling | M2 | 3–5 | 5–10 |
| KAN-3 | Caregiver Mobile App & EVV (GPS, Offline, HHAeXchange) | M3 | 6–9 | 11–18 |
| KAN-4 | Billing, Claims & Remittance (Waystar 837P/835) | M4 | 10–11 | 19–22 |
| KAN-5 | Reporting, AI Validation, UAT & Go-Live | M5 | 12–13 | 23–25 |
| KAN-6 | Platform Foundation — Azure, DevOps, UX & NFRs | cross-cutting | 1–13 | — |

## M1 — Core Multi-Tenancy, Security & Access Control (KAN-1)

| Key | Summary | Sprint | SOW ref |
|---|---|---|---|
| KAN-7 | Multi-tenant data architecture and tenant provisioning | 1 | N-01 |
| KAN-8 | Super Admin tenant management console | 1 | N-01 |
| KAN-9 | Per-tenant service module activation | 1 | N-02 |
| KAN-10 | Subscription and licence plan management with usage metrics | 1 | N-03 |
| KAN-11 | Unified user model and API gateway foundation | 1 | Core platform |
| KAN-12 | Authentication with ASP.NET Identity and JWT | 2 | C-01 |
| KAN-13 | Two-factor authentication (2FA) for web and mobile | 2 | C-01 |
| KAN-14 | Role-based access control for the six platform roles | 2 | N-04 |
| KAN-15 | Row-level security and data separation per TenantID | 2 | Data separation |
| KAN-16 | Audit logging framework for system events and PHI access | 2 | N-06, O-01, O-03 |
| KAN-17 | Agency user management for caregivers, schedulers, billers | 2 | A-01 |
| KAN-18 | Super Admin system monitoring and support management | 2 | N-05, N-07 |

## M2 — EHR Lite & Scheduling (KAN-2)

| Key | Summary | Sprint | SOW ref |
|---|---|---|---|
| KAN-19 | Client/patient registration and demographics | 3 | A-02 |
| KAN-20 | Caregiver management and credentialing with expiry tracking | 4 | A-01 |
| KAN-21 | Simplified care plan entry with task list | 4 | A-05, C-04 |
| KAN-22 | Service authorization management with rates and billing limits | 5 | A-03 |
| KAN-23 | Visit scheduling: create, edit and cancel visits | 5 | S-01, A-04 |
| KAN-24 | Caregiver shift assignment with conflict/eligibility checks | 5 | S-02 |
| KAN-25 | Scheduler calendar and roster views | 5 | S-01, S-02 |
| KAN-26 | Notification service for push, SMS and email alerts | 4 | C-08, S-05 |
| KAN-27 | Automated visit alerts for missed check-ins and overlaps | 5 | S-05 |
| KAN-28 | Real-time synchronisation with SignalR | 3 | Real-time comms |
| KAN-29 | Role-based dashboards for Admin, Scheduler, Biller, Auditor | 3 | Core platform |
| KAN-30 | Incident report capture and review | 4 | A-05, C-05, O-02 |

## M3 — Caregiver Mobile App & EVV (KAN-3)

| Key | Summary | Sprint | SOW ref |
|---|---|---|---|
| KAN-31 | Mobile app project setup, navigation shell and build pipeline | 6 | Mobile app |
| KAN-32 | Caregiver secure mobile login with 2FA and biometric unlock | 6 | C-01 |
| KAN-33 | EVV check-in and check-out with GPS capture | 6 | C-02 |
| KAN-34 | Geofence setup for authorised service locations | 7 | S-04 |
| KAN-35 | Geofence validation of check-in and check-out | 7 | C-02, S-04 |
| KAN-36 | Offline data capture in the mobile app | 7 | C-03 |
| KAN-37 | Offline sync engine with conflict resolution | 7 | C-03 |
| KAN-38 | Care plan and visit task access on mobile | 8 | C-04 |
| KAN-39 | Visit charting: progress notes, vitals and incidents | 8 | C-05 |
| KAN-40 | Client digital signature capture | 8 | C-06 |
| KAN-41 | Visit summary submission for approval and billing | 8 | C-07 |
| KAN-42 | Push notifications for visit reminders and schedule changes | 8 | C-08 |
| KAN-43 | HHAeXchange integration for EVV data exchange | 8 | Integration layer |
| KAN-44 | EVV monitoring dashboard for real-time check-in/out status | 9 | S-03 |
| KAN-45 | End-to-end EVV cycle QA and mobile release preparation (task) | 9 | — |

## M4 — Billing, Claims & Remittance (KAN-4)

| Key | Summary | Sprint | SOW ref |
|---|---|---|---|
| KAN-46 | Visit verification and approval workflow | 10 | S-06, A-06 |
| KAN-47 | Billing rules engine per service type | 10 | Billing rules |
| KAN-48 | Billing generation engine from approved visits | 10 | B-01 |
| KAN-49 | Waystar API integration for 837P claim submission | 11 | B-02 |
| KAN-50 | 835 ERA remittance import and payment posting | 11 | B-03 |
| KAN-51 | Payment tracking and invoice reconciliation | 11 | B-04 |
| KAN-52 | Billing exception handling and claim resubmission | 11 | B-05 |
| KAN-53 | Agency Admin billing review before submission to Waystar | 11 | A-06 |
| KAN-54 | Reporting data foundation and data audit checks | 11 | Initial reporting |

## M5 — Reporting, AI Validation, UAT & Go-Live (KAN-5)

| Key | Summary | Sprint | SOW ref |
|---|---|---|---|
| KAN-55 | EVV Compliance Report | 12 | O-02, A-07 |
| KAN-56 | Billing and Claims Summary Report | 12 | B-06, A-08 |
| KAN-57 | Payroll / Compensation Summary Report with export | 12 | MVP report 3 |
| KAN-58 | Visit Productivity Report | 12 | A-08 |
| KAN-59 | AI-assisted data validation rules (MVP) | 12 | AI validation engine |
| KAN-60 | Compliance monitoring dashboard and audit readiness view | 12 | A-07 |
| KAN-61 | Auditor portal: audit log, PHI access monitoring, read-only | 12 | O-01, O-03, O-05 |
| KAN-62 | Audit data export for state and federal audits | 12 | O-04 |
| KAN-63 | UAT execution and critical feedback resolution (task) | 13 | — |
| KAN-64 | Production deployment and go-live readiness (task) | 13 | — |
| KAN-65 | End-user training and documentation (task) | 13 | — |

## Platform Foundation — cross-cutting (KAN-6)

| Key | Summary | Type | Notes |
|---|---|---|---|
| KAN-66 | Azure infrastructure provisioning for dev, test, production | Task | Infra assumptions TBD in SOW |
| KAN-67 | CI/CD pipelines for API, web and mobile | Task | Azure DevOps vs GitHub Actions undecided |
| KAN-68 | Hangfire background job infrastructure | Story | |
| KAN-69 | UI/UX design system and high-fidelity screen designs | Task | |
| KAN-70 | Define and verify non-functional requirements | Task | SOW NFR table is empty (TBD) |
| KAN-71 | Obtain Waystar API credentials from the customer | Task | Blocks KAN-49, KAN-50 |
| KAN-72 | Obtain HHAeXchange EVV access from the customer | Task | Blocks KAN-43 |
| KAN-73 | HIPAA compliance review and security hardening | Task | |
| KAN-74 | Discovery: close out TBD assumptions and scope baseline | Task | |

## Open items raised from the documents

These were flagged on the tickets rather than decided unilaterally:

1. **Mobile framework** — the SOW offers "React Native/Flutter" as alternatives; one must be
   chosen before Sprint 6 (KAN-31, tracked in KAN-74).
2. **CI/CD platform** — "Azure DevOps or GitHub Actions" is still an either/or (KAN-67).
3. **Empty SOW tables** — every row of the Assumptions and Non-Functional Requirements tables
   is marked TBD; captured in KAN-74 and KAN-70.
4. **Timeline mismatch** — the SOW states a 4–6 month development timeline, while the milestone
   sheet plans 13 sprints across roughly 25 weeks (KAN-74).
5. **Customer dependencies** — Waystar credentials (needed by Sprint 11) and HHAeXchange access
   (needed by Sprint 8) are external blockers, linked as "blocks" in Jira (KAN-71, KAN-72).
6. **Data migration** — not mentioned anywhere in either document; if existing client, caregiver
   or authorization data must be migrated, that work is currently unscoped and unestimated (KAN-74).
7. **Service module coverage** — the SOW lists ten service modules; the milestone plan describes
   platform capability rather than per-module configuration and testing (KAN-74).

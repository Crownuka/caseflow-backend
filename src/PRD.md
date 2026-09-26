# CASEFLOW — Project Carter v1.0

## 1. Project Name & Description
**CASEFLOW** — a digital legal case-management and collaboration platform designed to centralize case information, improve court preparedness, support continuity between lawyers, reduce administrative burden, and provide clients with controlled visibility into their matters.

## 2. Project Vision
To create a centralized, mobile-first digital environment where a law firm's authorized lawyers and administrative staff can access and maintain up-to-date case information from anywhere, while clients receive appropriate visibility into their own matters.

The long-term vision is for CaseFlow to make the firm's knowledge about its cases institutional — rather than dependent on individual lawyers, physical files, diaries, or memory.

## 3. Problem Statement
Law firms often manage large numbers of cases using physical files, individual diaries, spreadsheets, messaging platforms, and information held only by individual lawyers or support staff.

This makes it difficult to know the current position of a matter, locate information quickly, track upcoming hearings, maintain continuity when a lawyer is unavailable, and ensure other lawyers are sufficiently informed to take over a matter at short notice. Clients also often experience limited visibility into the progress of their matters.

CaseFlow addresses these operational and information-management problems with a centralized digital system for case information, court dates, proceedings, documents, responsibilities, notifications, and controlled client communication.

## 4. Business/Product Objectives
1. Centralize the firm's case information
2. Improve lawyer preparedness for court appearances
3. Reduce avoidable failures from missed or poorly communicated hearing dates
4. Allow lawyers to access essential case information regardless of location
5. Reduce dependence on individual lawyers as sole holders of case knowledge
6. Reduce administrative information-management burden
7. Improve continuity when an assigned lawyer is unavailable
8. Give clients controlled and timely visibility into their matters
9. Create an environment where junior lawyers can learn from the firm's existing cases
10. Digitize important aspects of the firm's case-management workflow

## 5. Target Users

### Primary User 1 — Lawyer
- Access and search firm cases
- Review case history and proceedings
- See upcoming hearings
- Access relevant documents
- Receive notifications
- Update case information; create internal notes
- Identify the responsible lawyer
- Prepare to cover another lawyer's matter

### Primary User 2 — Admin/Secretary
- Create and maintain case records
- Maintain filing information; enter case and client information
- Record hearing dates; upload documents; enter judgments
- Maintain administrative information and organized digital records

### Primary User 3 — Client
- Access permitted case information
- View upcoming hearing dates; receive notifications
- View approved case updates
- Submit their own account of what happened in court (clearly flagged as client-sourced)

### Future Stakeholders (Out of MVP Scope)
- Court Registrar — potential future integration
- Judge — potential future integration

## 6. Proposed Solution
A centralized web application providing:
- Case management & history
- Lawyer assignment & responsibility tracking
- Hearing/calendar management & reminders
- Records of proceedings & documentation logs
- In-app/email notifications
- Internal lawyer secure notes
- Client-visible updates & reporting
- Global search & interactive dashboards
- Role-based access control (RBAC)

Designed for fluid access from phone, laptop, or other supported devices.

## 7. Scope Boundaries

### In Scope — MVP
- **Authentication:** Registration, login, logout, user roles
- **Case Management:** Create, view, edit, search cases; tracks status, practice area, court info, client links, assigned attorneys, chronological history
- **Hearing Management:** Add/update hearings, adjournments, next hearing dates, visual history, alerts, notifications
- **Lawyer Collaboration:** Firm-wide case visibility, granular responsibilities, status logs, internal notes, handover/cover workflows
- **Documents:** Secure uploads, categorization, linking files to cases/hearings
- **Client Portal:** Isolated login, permitted case visibility, timelines, hearing tracking, client-submitted accounts
- **Administration:** Baseline records, digital folder frameworks, admin management

### Out of Scope — Post-MVP
- Judge and Court Registrar portals
- Live API integration with external court systems
- Document filing automation
- Generative AI legal research/advice/predictions
- In-platform billing/payments
- Native mobile apps, embedded video conferencing
- Legal Reference Library (pending copyright/jurisdictional validation)

## 8. Success Criteria

**Operational:** fewer missed hearings; faster case-info retrieval; reduced reliance on physical files; clear file ownership and cover pathways

**Lawyer:** better court preparation; full calendar awareness; remote access to case data; junior lawyers can study historical files

**Management:** less time tracing updates manually; real-time caseload overview

**Client:** higher self-service satisfaction; less manual outreach for routine updates

## 9. Key Stakeholders
Principal/Managing Partner, Head of Chambers, Lawyers & Junior Lawyers, Admin/Secretary, Clients (all High Interest) — Court Registrars & Judges (Future Phase) — Development Team/Product Manager (High Interest)

## 10. Assumptions
- Firms are willing to migrate from paper to digital systems
- Users have consistent internet-connected device access
- Staff can be trained on the platform
- Firms have clear internal access-clearance rules
- Firms enter accurate data
- Clients will engage with a client portal
- The app can operate independently of court systems in early versions
- Role-based access safely segregates user paths
- Client entries are clearly distinct from attorney notes

## 11. Project Constraints
- **Technical:** Solo development with AI-assisted tooling; structure must stay legible for a solo developer, with low running costs
- **Financial:** Stay within free/low-tier hosting limits
- **Time:** Move quickly through planning to unlock AI-assisted build speed
- **Security:** Non-negotiable, given sensitive litigation data
- **Scope:** Actively guard against scope creep

## 12. Risk Register

| Risk | Impact | Initial Response |
|---|---|---|
| Scope becomes too large | High | Strict adherence to MVP boundaries |
| Incorrect requirements engineered | High | Iterative discovery and validation check-ins |
| Poor permission/role architecture | Very High | Formal role-mapping before coding |
| Confidential data breach | Very High | Security-by-design from Day 1 |
| Inaccurate case histories | High | Immutable database history logs |
| Client logs inaccurate claims | Med/High | Explicit verification warning stamps |
| Staff leaves platform idle | High | Accountability triggers, automated reminders |
| Firm resists adoption | High | Intuitive, minimalist UX |
| AI-generated code breaks | High | Rigorous manual testing and code review |

---
*Current status: Authentication module (register/login) implemented and tested. See [`README.md`](./README.md) for setup and current feature status.*
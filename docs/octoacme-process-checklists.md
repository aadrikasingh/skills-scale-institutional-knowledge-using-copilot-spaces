# OctoAcme — Process Checklists

Reusable checklists for the three most common cross-role handoff and gate moments. Copy the relevant checklist into your project notes or issue tracker for each occurrence.

For role ownership at each gate see the [RACI Matrix](./octoacme-raci-matrix.md). For full role descriptions see [Roles & Personas](./octoacme-roles-and-personas.md).

---

## 1. Kickoff Checklist (Initiation → Planning Handoff)

**Owner**: Project Manager — confirm each item before the kickoff meeting closes.

### Pre-kickoff (Initiation complete)
- [ ] Project One-pager reviewed and approved by Product Manager and Sponsor
- [ ] Business Analyst has documented high-level requirements or problem scope
- [ ] Key stakeholders identified and communication plan drafted
- [ ] Initial risk list created and added to Risk Register
- [ ] Team composition confirmed (roles filled: PM, PdM, Dev, BA, UX, Security Lead, DevOps, Release Manager as applicable)

### Kickoff meeting
- [ ] Problem statement and goals presented and agreed by all attendees
- [ ] Success metrics defined and accepted
- [ ] High-level timeline and milestones reviewed
- [ ] Roles and responsibilities confirmed (reference [Roles & Personas](./octoacme-roles-and-personas.md))
- [ ] RACI reviewed for this project (reference [RACI Matrix](./octoacme-raci-matrix.md))
- [ ] Definition of Done drafted or agreed

### Post-kickoff (Planning starts)
- [ ] Backlog seeded with initial user stories and acceptance criteria (led by Business Analyst + Product Manager)
- [ ] Design/UX track kicked off — UX Designer scheduled for research or wireframing
- [ ] Security requirements captured in backlog (Security Lead sign-off required)
- [ ] CI/CD baseline confirmed by DevOps Engineer
- [ ] Release calendar placeholder created by Release Manager
- [ ] Project board and repo skeleton set up

---

## 2. Release Readiness Checklist (Pre-release Gate)

**Owner**: Release Manager — all items must be confirmed before triggering deployment.

### Scope & quality
- [ ] All acceptance criteria for in-scope items are met
- [ ] All PRs merged to release branch; no open draft PRs for this release
- [ ] CI pipeline green (tests, lint, security scans)
- [ ] Security Lead has reviewed and signed off (no open critical/high vulnerabilities)
- [ ] UX Designer has reviewed implemented features against design specs (if applicable)
- [ ] Business Analyst has confirmed UAT completion and sign-off

### Deployment readiness
- [ ] Deployment window scheduled and communicated (DevOps Engineer)
- [ ] Staging deployment completed and smoke tests passed
- [ ] Rollback plan documented and tested (DevOps Engineer + Release Manager)
- [ ] Migration steps (DB, config, etc.) documented and reviewed
- [ ] Monitoring and alerting confirmed active for affected services (DevOps Engineer)

### Communication
- [ ] Release notes drafted and reviewed by Product Manager
- [ ] Stakeholder announcement prepared (release name, summary, notable changes)
- [ ] Support / on-call team notified of release scope and potential impact
- [ ] Post-deploy verification steps documented

### Go / No-go
- [ ] Release Manager calls go/no-go with PM, PdM, and Security Lead input
- [ ] Go decision recorded in the release notes or project log

---

## 3. Stakeholder Update Checklist (Weekly Status)

**Owner**: Project Manager — complete before sending the weekly status update.

### Gather inputs
- [ ] Progress this week collected from Developers, BA, and UX Designer
- [ ] Next steps confirmed with Product Manager for upcoming sprint
- [ ] Risks & blockers reviewed in Risk Register (Security Lead and DevOps Engineer consulted if relevant)
- [ ] Decisions needed identified and owners confirmed

### Draft and review
- [ ] Status update drafted using the Weekly Status Template (see [Risks & Communication](./octoacme-risks-and-communication.md))
- [ ] Release Manager adds release schedule updates if applicable
- [ ] Update reviewed by Product Manager before sending

### Send and log
- [ ] Update distributed to the stakeholder list on file
- [ ] Update archived in the project repo or shared drive (single source of truth)
- [ ] Any decisions made in response to the update are logged in the decision log

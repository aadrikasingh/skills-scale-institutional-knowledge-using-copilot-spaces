# OctoAcme Project Management Docs

This folder is the single entry point for OctoAcme project management documentation. It covers the full project lifecycle, team roles, communication strategies, and quality practices used across all cross-functional product deliveries.

## Overview

OctoAcme runs projects using a lightweight, repeatable lifecycle that emphasises clear ownership, iterative delivery, and measurable outcomes. Work moves through five stages: **Initiation** (clarify the problem, goals, success metrics, stakeholders, and a high-level timeline), **Planning** (break work into shippable increments, define acceptance criteria and a Definition of Done, and map milestones and releases), **Execution** (build, test, and review in small increments), **Release** (deploy with verification and rollback readiness), and **Close/Retro** (capture learnings and convert them into tracked improvements). Across all stages the guiding principles are customer-first delivery, transparency, and data-informed decisions.

Roles are explicitly defined to keep accountability clear. The **Project Manager (PM)** coordinates delivery logistics — timelines, risk management, meeting facilitation, and stakeholder communications — while the **Product Manager (PdM/Product Lead)** defines outcomes, prioritises the backlog, and measures success against metrics. **Developers** design and implement changes with testability and maintainability in mind, collaborating through code reviews and estimation. **QA/Testing** supports feature validation and acceptance, and **stakeholders/sponsors** provide input, approvals, and escalation support when business-impacting issues arise.

Execution is driven by a consistent team rhythm. Teams maintain a project board (e.g., GitHub Projects) with stages such as Backlog → Ready → In Progress → In Review → QA → Done, and hold daily standups plus a weekly delivery sync to demo progress and surface risks. Communication is structured and predictable: PM/PdM alignment happens weekly, delivery teams hold standups as agreed, and stakeholders receive periodic updates in a standard status format (progress, next steps, risks/blockers, and decisions needed). Blockers escalate in tiers — from team triage, to PM + Product Lead + dependent teams, and ultimately to sponsor-level escalation for major business impact.

Quality assurance is built into both day-to-day execution and release readiness. The team favours smaller pull requests, links work back to issues and acceptance criteria, runs CI checks (tests, lint, security scanning), and requires at least one approval before merge. Testing expectations include unit tests for new logic, integration tests where appropriate, and end-to-end smoke tests for critical flows. Releases follow a standardised checklist — acceptance criteria met, CI/security scans passing, release notes prepared, and rollback/mitigation plans in place — with deployments moving through staging validation, production rollout, post-deploy verification, and stakeholder announcement.

## Process Documents

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risks & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [RACI Ownership Matrix](./octoacme-raci-matrix.md)
- [Process Checklists](./octoacme-process-checklists.md)

# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
Release Managers own end-to-end release planning, coordination, and communication. They ensure releases are well-scoped, properly gated, and delivered with minimal disruption.

### Responsibilities
- Maintain the release calendar and coordinate deployment windows
- Drive the release readiness gate: verify all acceptance criteria, CI scans, and rollback plans are in place
- Draft and distribute release notes and stakeholder announcements
- Coordinate with on-call and support teams before each release
- Own the rollback decision and incident escalation during deployments

### Goals
- Ship reliably and predictably with minimal production incidents
- Keep all stakeholders informed before, during, and after releases
- Continuously improve deployment speed and safety

### Typical Communication
- Pre-release readiness checklist shared with the delivery team (see [Process Checklists](./octoacme-process-checklists.md))
- Release notes and announcements to stakeholders
- Incident notifications and post-deploy status updates

### Interactions with Existing Roles
- **Developers**: confirms all PRs are merged, CI is green, and migration steps are documented
- **Product Managers**: aligns on release scope, messaging, and go/no-go decision
- **Project Managers**: coordinates timeline, deployment windows, and risk register updates

---

## UX Designer

### Role Summary
UX Designers champion the end-user experience throughout the product lifecycle. They translate user needs into clear design artifacts and validate solutions with real users before and after launch.

### Responsibilities
- Conduct user research and usability testing to inform design decisions
- Produce wireframes, prototypes, and design specifications
- Define and maintain UX acceptance criteria alongside functional criteria
- Participate in backlog refinement to flag usability risks early
- Review implemented features against designs before release

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce rework by catching usability issues before implementation begins
- Establish a shared design language (component library or style guide)

### Typical Communication
- Design reviews with Product Managers and Developers during planning and sprint kickoffs
- Usability test findings shared as concise summaries or annotated recordings
- Design files and specifications linked in backlog items

### Interactions with Existing Roles
- **Developers**: provides design specs, answers implementation questions, reviews UI in PR reviews or staging builds
- **Product Managers**: collaborates on problem framing, feature scoping, and success metrics tied to user experience
- **Project Managers**: flags design dependencies and usability research windows in the project plan

---

## Security Lead

### Role Summary
The Security Lead ensures that security considerations are built into every phase of the project lifecycle — not treated as a last-minute gate. They own the security posture of delivered systems and coordinate response when vulnerabilities are discovered.

### Responsibilities
- Define and maintain security requirements and acceptance criteria
- Review architecture and design decisions for security risks
- Ensure security scanning (SAST, dependency checks) is active in CI
- Triage and prioritise identified vulnerabilities; track remediation in the risk register
- Lead security incident response and post-incident reviews
- Maintain the security incident runbook referenced in [Risks & Communication](./octoacme-risks-and-communication.md)

### Goals
- Prevent vulnerabilities from reaching production
- Reduce mean-time-to-detect and mean-time-to-remediate security issues
- Build a security-aware culture across the delivery team

### Typical Communication
- Security review sign-off as part of release readiness (see [Process Checklists](./octoacme-process-checklists.md))
- Vulnerability triage summaries shared with Project Managers and Developers
- Incident communications following the template in [Risks & Communication](./octoacme-risks-and-communication.md)

### Interactions with Existing Roles
- **Developers**: reviews code for security anti-patterns, provides remediation guidance, approves security-sensitive PRs
- **Product Managers**: advises on the risk/cost trade-off of deferring security work
- **Project Managers**: ensures security tasks are tracked in the backlog and risk register with owners and due dates

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the delivery infrastructure that enables the team to ship safely and frequently. They bridge development and operations, prioritising automation, reliability, and fast feedback.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines
- Manage cloud infrastructure, environments, and access controls
- Define and enforce branching, deployment, and rollback procedures
- Monitor system health, set up alerting, and respond to operational incidents
- Collaborate on the Definition of Done to include deployability and observability requirements

### Goals
- Reduce deployment lead time and failure rate
- Maximise system availability and observability
- Automate toil so developers can focus on feature delivery

### Typical Communication
- Pipeline and infrastructure runbooks linked from [Execution & Tracking](./octoacme-execution-and-tracking.md)
- Incident notifications and post-mortem action items
- Capacity and environment updates during sprint planning or weekly delivery syncs

### Interactions with Existing Roles
- **Developers**: pairs on pipeline configuration, reviews infrastructure-as-code PRs, supports local environment issues
- **Product Managers**: communicates infrastructure constraints that may affect delivery timelines or feature feasibility
- **Project Managers**: flags environment risks, deployment dependencies, and capacity concerns in the project plan; supports release window scheduling with Release Managers

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business stakeholders and the delivery team. They elicit, document, and validate requirements so that what gets built aligns with real business needs.

### Responsibilities
- Facilitate requirements workshops and stakeholder interviews
- Translate business needs into user stories, process maps, and acceptance criteria
- Maintain traceability between business goals and backlog items
- Identify gaps, conflicts, or ambiguities in requirements early
- Support UAT planning and sign-off

### Goals
- Ensure delivered features solve the right business problems
- Reduce rework caused by misunderstood or missing requirements
- Improve stakeholder confidence through clear documentation and regular validation

### Typical Communication
- Requirements documentation and process-flow diagrams shared at planning kickoffs
- Acceptance criteria co-authored with Product Managers and added to backlog items
- UAT reports and sign-off shared with Project Managers before release

### Interactions with Existing Roles
- **Developers**: clarifies requirements during refinement, answers implementation questions, validates edge cases
- **Product Managers**: co-owns the backlog — BAs provide requirements depth while PdMs own prioritisation and strategy
- **Project Managers**: ensures requirements milestones (workshops, sign-offs) are reflected in the project plan and tracked against timelines

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See the [RACI Matrix](./octoacme-raci-matrix.md) for a cross-role ownership view of key artifacts and activities.
- See [Process Checklists](./octoacme-process-checklists.md) for reusable kickoff, release readiness, and stakeholder update checklists.


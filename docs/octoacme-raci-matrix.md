# OctoAcme — RACI Ownership Matrix

This matrix maps core project artifacts and activities to team roles using a lightweight RACI model.

> **R** = Responsible (does the work) · **A** = Accountable (final decision/sign-off) · **C** = Consulted (provides input) · **I** = Informed (kept up to date)

For full role descriptions see [Roles & Personas](./octoacme-roles-and-personas.md).

---

## Artifact & Activity Ownership

| Artifact / Activity          | Project Manager | Product Manager | Developers | Release Manager | UX Designer | Security Lead | DevOps Engineer | Business Analyst |
|------------------------------|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Project One-pager / Charter  | A | R | I | I | C | C | I | C |
| Backlog & Prioritization     | C | A | C | I | C | C | I | R |
| Definition of Done (DoD)     | A | C | R | C | C | C | C | C |
| Risk Register                | A | C | C | C | I | R | C | C |
| Release Plan / Calendar      | C | C | C | A | I | C | R | I |
| Stakeholder Updates          | A | C | I | C | I | I | I | C |
| Incident Communications      | C | I | C | C | I | A | R | I |
| Retro Action Items           | A | C | R | I | C | C | C | C |
| Security Review Sign-off     | I | I | C | C | I | A | C | I |
| UX / Design Specs            | I | C | C | I | A | I | I | C |
| CI/CD Pipeline               | I | I | C | C | I | C | A | I |
| Requirements / User Stories  | C | A | C | I | C | C | I | R |
| UAT Sign-off                 | C | A | I | C | C | C | I | R |

---

## Notes
- Accountability (A) should map to exactly one owner per row where possible. If ownership is genuinely shared, note it explicitly.
- This matrix is a starting point; adapt it to your project's actual team composition.
- Review and update this matrix at project kickoff and after significant scope changes.
- Cross-reference with checklists in [Process Checklists](./octoacme-process-checklists.md) to confirm ownership at each gate.

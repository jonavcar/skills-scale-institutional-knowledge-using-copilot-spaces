# OctoAcme — Quality & Release Readiness Checklist

## Purpose
Provide a shared checklist that the QA Lead and Release Manager complete together before any release proceeds. Referencing artifacts already tracked in the project (acceptance criteria, Definition of Done, risk register, release notes, rollback plan) ensures nothing is missed and ownership is explicit.

**Owners:** QA Lead (quality sections) · Release Manager (deployment & communication sections)

---

## 1 — Requirements & Acceptance Criteria

| # | Check | Owner | Status |
|---|-------|-------|--------|
| 1.1 | All acceptance criteria for in-scope backlog items are documented and approved | Business Analyst / PdM | ☐ |
| 1.2 | Acceptance criteria have been reviewed by QA Lead for testability | QA Lead | ☐ |
| 1.3 | Any out-of-scope items or deferred stories are captured and communicated | PM | ☐ |

---

## 2 — Quality & Testing

| # | Check | Owner | Status |
|---|-------|-------|--------|
| 2.1 | All acceptance criteria are covered by test cases (manual or automated) | QA Lead | ☐ |
| 2.2 | Unit and integration tests pass in CI | Developers | ☐ |
| 2.3 | End-to-end / smoke tests pass on the staging environment | QA Lead | ☐ |
| 2.4 | Security scanning in CI shows no new critical/high findings | Developers / QA Lead | ☐ |
| 2.5 | All blocker and critical defects are resolved or have an accepted mitigation | QA Lead | ☐ |
| 2.6 | Quality metrics (defect count, test coverage) reviewed and meet team thresholds | QA Lead | ☐ |
| 2.7 | Definition of Done satisfied for all items moving to Done | QA Lead | ☐ |
| 2.8 | UX/UI acceptance criteria verified against approved designs | QA Lead / UX/UI Designer | ☐ |

**QA Sign-off:** _______________________ Date: ___________

---

## 3 — Release Planning & Coordination

| # | Check | Owner | Status |
|---|-------|-------|--------|
| 3.1 | Deployment window scheduled and communicated to the team and stakeholders | Release Manager | ☐ |
| 3.2 | Release notes drafted, reviewed, and approved | Release Manager / PdM | ☐ |
| 3.3 | Rollback / mitigation plan is documented and accessible | Release Manager / PM | ☐ |
| 3.4 | Risk register reviewed; no unmitigated high-impact risks remain open | PM | ☐ |
| 3.5 | Merge freeze window confirmed with development team | Release Manager | ☐ |
| 3.6 | All PRs for this release are merged; no outstanding code changes | Developers | ☐ |

---

## 4 — Deployment Execution

| # | Check | Owner | Status |
|---|-------|-------|--------|
| 4.1 | Deployed to staging and smoke tests passed | Release Manager / QA Lead | ☐ |
| 4.2 | Backup or snapshot taken (if applicable) | Release Manager | ☐ |
| 4.3 | Deployed to production via automated pipeline (preferred) | Release Manager | ☐ |
| 4.4 | Post-deploy verifications completed | Developers / QA Lead | ☐ |
| 4.5 | Monitoring dashboards confirm healthy signals (errors, latency, usage) | Developers / Release Manager | ☐ |

---

## 5 — Stakeholder Communication

| # | Check | Owner | Status |
|---|-------|-------|--------|
| 5.1 | Release announced to stakeholders and support teams | Release Manager | ☐ |
| 5.2 | Known issues communicated with workarounds (if any) | Release Manager / PM | ☐ |
| 5.3 | Post-release metrics and incident summary shared with team (within 24–48 h) | Release Manager | ☐ |

---

## Release Sign-off

| Role | Name | Sign-off | Date |
|------|------|----------|------|
| QA Lead | | | |
| Release Manager | | | |
| Project Manager | | | |

---

*Related documents:*
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Project Planning](./octoacme-project-planning.md)

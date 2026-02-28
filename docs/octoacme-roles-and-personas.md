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

## Business Analyst

### Role Summary
Translates business requirements into actionable deliverables and ensures alignment between stakeholders, Product Managers, and technical teams.

### Responsibilities
- Elicit, document, and validate business and functional requirements
- Facilitate requirements workshops and backlog refinement sessions
- Map business processes and data flows to inform design and development
- Define acceptance criteria in collaboration with Product Managers and QA Lead
- Review and sign off on completed features against documented requirements

### Goals
- Ensure requirements are complete, unambiguous, and testable before development begins
- Reduce rework by catching misaligned expectations early
- Bridge communication gaps between business stakeholders and technical teams

### Typical Communication
- Requirements documents, user stories, and process flow diagrams
- Participation in sprint planning, backlog refinement, and acceptance reviews
- Email/chat updates to Product Managers on requirements changes

### Typical Interactions
- **Product Managers (PdM):** Collaborates to refine requirements, align on priorities, and confirm business value before items enter the sprint backlog.
- **Developers:** Provides business context and clarifies requirements during implementation; reviews deliverables for requirement conformance.
- **QA Lead:** Jointly defines and validates acceptance criteria; supports test case creation to ensure coverage of business rules.
- **Project Managers (PM):** Reports on requirement scope changes that may affect timelines or risk register.
- **Stakeholders:** Elicits requirements and manages expectation alignment throughout the project lifecycle.

---

## UX/UI Designer

### Role Summary
Advocates for user-centered design and ensures usability best practices inform development. Creates the visual and interaction design that bridges user needs with technical implementation.

### Responsibilities
- Create wireframes, mockups, and interactive prototypes
- Conduct usability reviews and validate design decisions with stakeholders or users
- Define and maintain the design system and style guidelines
- Collaborate with developers during implementation to ensure design fidelity
- Contribute to acceptance criteria related to UX/UI quality

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce development rework by providing clear, complete design specs
- Ensure design decisions are informed by user research and data

### Typical Communication
- Design files, annotated mockups, and prototypes shared via design tools
- Participation in sprint planning, backlog refinement, and design reviews
- Handoff notes and design specs for developers

### Typical Interactions
- **Product Managers (PdM):** Receives feature requirements and user research inputs; validates designs against product goals before development begins.
- **Developers:** Hands off design specs and provides clarification during implementation; reviews implemented UI for fidelity.
- **QA Lead:** Collaborates on UX acceptance criteria; QA Lead validates UI against approved designs and flags deviations.
- **Business Analyst:** Aligns on user workflow requirements and business process flows that inform interaction design.
- **Stakeholders:** Presents prototypes and design rationale for feedback and approval.

---

## QA Lead

### Role Summary
Oversees testing strategy, quality standards, and drives test planning and execution across the project lifecycle. Acts as the quality gate before release.

### Responsibilities
- Define and maintain the test strategy, test plan, and coverage requirements
- Coordinate manual and automated test execution (unit, integration, end-to-end)
- Validate that acceptance criteria are met before items move to Done
- Report quality metrics (defect counts, test coverage, open blockers) to the project team
- Own the QA column on the project board; move items to Done only when quality criteria are satisfied
- Contribute to release readiness sign-off alongside the Release Manager
- Maintain and execute the [Quality & Release Readiness Checklist](./octoacme-quality-and-release-readiness-checklist.md)

### Goals
- Prevent defects from reaching production
- Ensure every release meets the Definition of Done and acceptance criteria
- Provide the team with actionable quality signals throughout the sprint

### Typical Communication
- Test plans, defect reports, and quality dashboards
- QA status updates in weekly delivery syncs and sprint reviews
- Sign-off comments on PRs and project board items

### Typical Interactions
- **Developers:** Reviews defects and collaborates on root cause; verifies fixes before closing issues; participates in code and PR reviews for testability.
- **Product Managers (PdM):** Validates that acceptance criteria are testable; signals when quality thresholds are met (or not) prior to release.
- **Project Managers (PM):** Provides QA status and risk signals that feed into release readiness and the risk register.
- **Business Analyst:** Uses acceptance criteria defined by BA to build test cases; raises ambiguities back to BA before testing begins.
- **Release Manager:** Completes the quality portion of the [Quality & Release Readiness Checklist](./octoacme-quality-and-release-readiness-checklist.md) and provides formal QA sign-off before a release proceeds.

---

## Release Manager

### Role Summary
Ensures software releases are planned, coordinated, and communicated smoothly across engineering, QA, and business stakeholders. Owns the end-to-end release process.

### Responsibilities
- Plan and schedule deployment windows in coordination with the project team and stakeholders
- Own and execute the [Quality & Release Readiness Checklist](./octoacme-quality-and-release-readiness-checklist.md) prior to each release
- Ensure release notes are drafted, reviewed, and published
- Confirm rollback and mitigation plans are in place before deployment
- Coordinate with QA Lead to obtain formal release readiness sign-off
- Communicate release status, scope, and timelines to stakeholders and support teams
- Track and report post-release metrics and incidents back to the team

### Goals
- Deliver releases with minimal disruption and risk
- Maintain a predictable, documented release cadence
- Ensure all stakeholders are informed and aligned before and after each release

### Typical Communication
- Release schedule and deployment window notifications
- Release notes and post-release announcements
- Incident reports and rollback notifications when required

### Typical Interactions
- **Project Managers (PM):** Aligns release windows with project milestones and risk register; escalates release blockers through PM.
- **QA Lead:** Obtains QA sign-off via the [Quality & Release Readiness Checklist](./octoacme-quality-and-release-readiness-checklist.md) before any release proceeds.
- **Developers:** Coordinates deployment steps, confirms merge freeze windows, and validates that hotfixes or final PRs are merged.
- **Product Managers (PdM):** Confirms that release scope matches approved features; aligns on release notes content.
- **Stakeholders:** Communicates release timelines, notable changes, and any known issues ahead of and following deployment.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For handoff and quality/release processes, see the [Quality & Release Readiness Checklist](./octoacme-quality-and-release-readiness-checklist.md).


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

## Additional Personas (Recommended Additions)

These personas extend the core roles and clarify ownership across common cross-cutting concerns. Each persona includes responsibilities and how they interact with existing roles (PM, PdM, Developers, QA).

### Tech Lead / Engineering Lead
- Responsibilities:
  - Provide technical direction and architecture guidance.
  - Review complex design proposals and approve major technical decisions.
  - Mentor engineers and champion engineering quality and maintainability.
  - Identify technical risks and recommend mitigations.
- Interaction:
  - Works closely with Developers on design and implementation and leads technical code reviews.
  - Advises PdM and PM on feasibility, technical debt, and delivery risk.
  - Coordinates with QA on testability and non-functional requirements (performance, reliability).

### UX Designer / Product Designer
- Responsibilities:
  - Lead user research and synthesize findings into design recommendations.
  - Produce wireframes, interaction flows, and high-fidelity designs.
  - Define usability acceptance criteria and validate solutions with prototypes.
  - Maintain design system artifacts and accessibility guidance.
- Interaction:
  - Partners with PdM to shape product outcomes and success metrics.
  - Hands off assets, acceptance criteria, and interaction notes to Developers and QA.
  - Participates in demos, user-acceptance testing, and retrospectives to close the design loop.

### Security Engineer / Security Reviewer
- Responsibilities:
  - Run threat modeling and security reviews for significant changes.
  - Define security acceptance gates and CI checks (SAST, dependency scanning).
  - Triage security findings and provide remediation guidance.
  - Maintain security runbooks and incident escalation guidance.
- Interaction:
  - Reviews designs with the Tech Lead and Developers, and marks security gates for releases.
  - Informs PM about release constraints where security remediation is required.
  - Works with QA to ensure security regression tests and post-deploy monitoring are in place.

### Release / Platform Engineer
- Responsibilities:
  - Maintain CI/CD pipelines and deployment automation.
  - Run release rehearsals and manage rollback/migration procedures.
  - Define runbooks for deploy, rollback, and operational handoffs.
  - Improve platform observability and deployment reliability.
- Interaction:
  - Coordinates deployment windows and cutover steps with the Project Manager.
  - Supports Developers during release and provides staging environments for QA validation.
  - Works with Data/Analytics and Security to ensure monitoring and compliance checks are active.

### Data / Analytics Engineer or Analyst
- Responsibilities:
  - Define instrumentation and event schemas required for product metrics.
  - Ensure accurate capture and storage of analytics events.
  - Build dashboards and alerts used to validate release success metrics.
  - Support experiment instrumentation and metric definitions.
- Interaction:
  - Collaborates with PdM to define success metrics and measurement plans.
  - Supplies Developers with schemas and assists QA with metric-based validation.
  - Provides artifacts and analysis for retrospectives and post-release reviews.

### Customer Success / Support Representative
- Responsibilities:
  - Surface customer feedback and operational issues to the delivery team.
  - Help prioritize user-impacting bugs and coordinate customer communications.
  - Provide reproduction steps and context for support cases.
- Interaction:
  - Works with PdM to feed prioritization and with PM on customer-facing timelines.
  - Coordinates with Developers and QA to confirm fixes and validate patches.
  - Engages in release readiness checks when customer-facing changes are involved.

### Compliance / Legal Liaison (if applicable)
- Responsibilities:
  - Review regulatory impacts and approve data-handling changes.
  - Provide compliance checklists and gating criteria for regulated features.
  - Ensure documentation and release notes meet regulatory requirements.
- Interaction:
  - Engages PdM and PM early in planning for features touching regulated data.
  - Reviews release artifacts and may gate production deployment until compliance checks are satisfied.
  - Works with Security and Data/Analytics on audit trails and retention policies.

---

## How to Use These Personas

- In planning and backlog refinement, explicitly note which specialized personas should be consulted or will own specific acceptance criteria, runbooks, or validation steps.
- For releases, ensure the Release/Platform Engineer, Security Engineer, and Data/Analytics representatives are scheduled for rehearsal and signoffs as applicable.
- During incidents, route role-specific tasks (security triage, platform rollback, customer comms) to the named personas to speed resolution.
- Add these personas to onboarding materials so new team members understand who to contact for architecture, design, security, releases, analytics, and customer issues.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

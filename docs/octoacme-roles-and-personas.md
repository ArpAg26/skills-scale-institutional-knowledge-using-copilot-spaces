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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional personas (proposed)

Below are suggested additions to clarify ownership of cross-cutting activities (releases, security, observability, research, support, accessibility). For each persona: Role summary, Responsibilities, and Interactions with existing roles.

### Release Engineer
- Role summary: Owns release pipelines, deployment automation, and rollback procedures.
- Responsibilities:
  - Maintain CI/CD pipelines and release automation.
  - Coordinate deployment windows and run pre/post-deploy checks.
  - Maintain rollback plans and runbooks.
  - Verify release artifacts, tagging, and release notes.
  - Work with infrastructure teams on deployment-related changes.
- Interactions:
  - Works with Project Manager to schedule windows and risk communications.
  - Coordinates with Developers for build artifacts and release readiness.
  - Partners with QA to validate staging and run smoke tests.
  - Aligns with Product on release readiness and announcement content.

### UX Researcher
- Role summary: Designs and runs user research to validate assumptions and inform product decisions.
- Responsibilities:
  - Plan and conduct research studies (interviews, usability tests, surveys).
  - Synthesize findings into actionable insights and recommendations.
  - Produce personas, journey maps, and prioritized research outputs.
  - Recommend acceptance criteria or design changes based on evidence.
- Interactions:
  - Partners with Product Manager to define research questions and success criteria.
  - Works with Designers on prototypes and test materials.
  - Shares findings with Developers and QA to inform acceptance test scenarios.

### Data Analyst
- Role summary: Measures product usage and defines metrics to validate success criteria.
- Responsibilities:
  - Define instrumentation requirements and tracking plans.
  - Create dashboards, run analyses, and validate experiment results.
  - Recommend metric-driven prioritization and success thresholds.
  - Support measurement of A/B tests and feature impact.
- Interactions:
  - Works with Product Manager to define success metrics and dashboards.
  - Collaborates with Developers/QA on instrumentation and telemetry.
  - Provides reports to PMs and stakeholders for decision-making.

### Security Engineer
- Role summary: Ensures security considerations are integrated into design, implementation, and release.
- Responsibilities:
  - Conduct threat modeling and security reviews for features.
  - Review PRs for security implications and run automated scans.
  - Advise on mitigations and emergency response for security incidents.
  - Maintain security checklists for releases.
- Interactions:
  - Collaborates with Developers during design and code review.
  - Coordinates with Release Engineer on deployment hardening.
  - Communicates risks and mitigations to PM/Project Manager.

### Observability Engineer
- Role summary: Defines monitoring, logging, and alerting standards that make systems operable.
- Responsibilities:
  - Design telemetry and logging standards.
  - Configure dashboards and alerts (SLO/SLI).
  - Triage monitoring gaps and tune alerts to reduce noise.
  - Create/runbook guidance for on-call responders.
- Interactions:
  - Works with Developers to instrument code and define metrics.
  - Partners with Data Analyst on metric definitions and dashboards.
  - Supports Support/On-call teams with runbooks and incident context.

### Customer Success / Support Liaison
- Role summary: Represents customer-facing teams to ensure feedback and incidents inform backlog and priorities.
- Responsibilities:
  - Triage incoming customer issues and surface recurring problems.
  - Track support trends, severity, and escalations.
  - Coordinate communications for major incidents and follow-ups.
  - Provide context and reproduction steps to Engineering and QA.
- Interactions:
  - Escalates production issues to Project Manager and Release Engineer.
  - Provides product usage context to Product Manager to inform prioritization.
  - Works with QA to reproduce and validate fixes.

### Accessibility Advocate
- Role summary: Ensures accessibility requirements are considered throughout design and development.
- Responsibilities:
  - Define accessibility acceptance criteria and test approaches.
  - Perform audits and provide remediation guidance.
  - Maintain a checklist of critical accessibility checks.
- Interactions:
  - Works with Designers on accessible designs.
  - Partners with Developers and QA to include accessibility in acceptance criteria and regression tests.

---

## Using these personas together
- Add the owning persona to relevant issues and PRs (e.g., "Observability Engineer — instrumentation", "Release Engineer — release readiness").
- Use the Acceptance Criteria template (where relevant) to call out responsibilities for cross-cutting activities (security checks, telemetry, accessibility).
- For onboarding, link each persona in the project README and add pointers to checklists (release, observability, security) stored in docs/.

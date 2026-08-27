# OctoAcme Project Management Documentation

## Overview
OctoAcme uses a structured, iterative approach to project management that emphasizes customer value, clear ownership, and data-informed decisions. The process spans five phases: Initiation, Planning, Execution, Release, and Continuous Improvement.

Projects begin with a lightweight Project One-pager to validate the business need, success criteria, and stakeholders. During Planning the team breaks work into shippable backlog items with clear acceptance criteria and a Definition of Done. Execution follows an iterative cadence with visible work on a project board and disciplined pull-request practices. Releases are staged with pre-release checks and rollback plans, and every workstream ends with a retrospective to capture learnings and convert them into tracked improvements.

OctoAcme’s approach balances predictable delivery with flexibility to iterate: small, testable increments reduce risk and enable faster feedback, while defined decision gates and stakeholder alignment keep projects focused on measurable outcomes.

## Key Workflows
- Project lifecycle: Initiation → Planning → Execution → Release → Retrospective
- Project board workflow: Backlog → Ready → In Progress → In Review → QA → Done
- Pull requests: keep PRs small (≤ 400 lines when possible), include issue links and acceptance criteria, run automated tests and linting in CI, and require at least one approval before merging
- Risk management: maintain a Risk Register with impact, likelihood, owner, and mitigation; escalate blockers via defined paths (Team → PM → Product Lead → Sponsor)

## Personas & Roles
- Project Manager (PM): coordinates delivery, risk management, scheduling, and stakeholder communication
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success using identified metrics
- Developers: implement features, write tests, and participate in reviews
- QA/Testing: validate acceptance criteria and perform manual or automated testing where required
- Stakeholders & Sponsors: provide approvals and business context

## Communication & Cadence
- Daily standups (15 minutes) for progress and blockers
- Weekly delivery sync to show progress, raise risks, and align on dependencies
- Demo/Review at the end of each sprint or milestone
- Monthly stakeholder updates and ad-hoc escalations as needed

## Quality Assurance Practices
- Unit and integration tests for new logic
- End-to-end smoke tests for critical flows before release
- Security scanning integrated into CI pipelines
- Manual QA for feature acceptance when needed
- Use dashboards and metrics to monitor release health and key signals (errors, latency, usage)

## Documentation Index
- Core Guidance
  - [Project Management Overview](octoacme-project-management-overview.md)

- Process Guides by Phase
  1. Initiation - [Project Initiation Guide](octoacme-project-initiation.md)
  2. Planning - [Project Planning](octoacme-project-planning.md)
  3. Execution - [Execution & Tracking](octoacme-execution-and-tracking.md)
  4. Release - [Release & Deployment Guide](octoacme-release-and-deployment.md)
  5. Improvement - [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

- Supporting Resources
  - [Risk Management & Communication](octoacme-risks-and-communication.md)
  - [Roles & Personas](octoacme-roles-and-personas.md)

## How to Use These Docs
- Keep the Project One-pager and project README updated in your project repo
- Reference the relevant phase guide based on the project stage
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context
- Use the `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml` template to propose changes to these docs


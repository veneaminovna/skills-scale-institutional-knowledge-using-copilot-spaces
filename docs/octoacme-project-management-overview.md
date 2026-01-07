# OctoAcme Project Management Docs

This README is the central entry point to OctoAcme’s project management process documentation. It orients new contributors, explains key workflows and roles, and links to the full set of living program documents in this folder.

---

## Overview: How OctoAcme Runs Projects

OctoAcme adopts an iterative, outcome-focused approach to delivering projects. Each project follows a lifecycle that starts with a clear initiation (Project One‑pager and stakeholder alignment), proceeds through detailed planning (backlog, estimates, Definition of Done, release map), goes into structured execution with tracked delivery and QA, advances through a checklist-driven release and deployment stage, and concludes with a close and retrospective. Key artifacts are maintained in the repo as the single source of truth.

**Core roles and responsibilities:**  
- **Product Managers (PdMs):** Define outcomes, prioritize, and measure success.
- **Project Managers (PMs):** Coordinate delivery, risk, and communication.
- **Developers:** Implement and test solutions and collaborate on design.
- **QA:** Validate acceptance criteria and orchestrate test coverage.
- **Release Managers:** Coordinate release activities, schedules, and deployment processes.
- **Risk & Compliance Leads:** Identify and mitigate risks, ensure compliance with standards.
- **Technical Architects:** Design system architecture and guide technical decisions.
- **Change Managers:** Manage change requests and ensure smooth process transitions.
- **External Stakeholders:** Provide input and validate deliverables according to business needs.

For detailed role descriptions and interactions, see [Roles & Personas](./octoacme-roles-and-personas.md).

**Workflows and quality assurance:**  
- Use a project board (Backlog → Ready → In Progress → In Review → QA → Done).
- Small pull requests; issue links and clear acceptance criteria required.
- Tests and security scans run in CI before review; PRs require approval(s).
- Release is checklist-driven with pre-release verifications and rollback plans.
- Blocker/risk escalation steps from daily team triage up to sponsor level.
- Quality is embedded by continuous testing, manual QA, and blameless retrospectives.

**Communication:**  
- Daily standups (progress + blockers), weekly PM/PdM syncs, sprint demos, and monthly stakeholder updates.
- Use templates for weekly updates and post-incident communications to maintain transparency.
- The project repo’s README and release docs act as status references for stakeholders.

**Continuous improvement:**  
- Retrospectives after each major deliverable.
- Action items tracked on project board and fed back into process documentation.

---

## Documentation Index

### Core Process Documentation
- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

### Templates & Checklists
- [Role Onboarding Checklist](./role-onboarding-checklist.md)
- [Risk Escalation Path Template](./risk-escalation-path-template.md)
- [Release Manager Checklist](./release-manager-checklist.md)

---

## How to Use

- Treat the docs in this folder as your reference for running projects at OctoAcme.
- Use templates and checklists as the basis for planning, releases, and retrospectives.
- To propose updates, use the issue template: `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml`.
- Add project-specific process artifacts to `.copilot/` if you want Copilot Spaces to use them as context.

---

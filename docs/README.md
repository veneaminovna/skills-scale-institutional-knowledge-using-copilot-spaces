# OctoAcme Project Management Docs

This README is the central entry point to OctoAcme's project management process documentation. It orients new contributors, explains key workflows and roles, and links to the full set of living program documents in this folder.

---

## Overview: How OctoAcme Runs Projects

OctoAcme runs projects with a lightweight, iterative lifecycle that begins with clear initiation (Project One‑pager, stakeholder alignment), moves into structured planning (kickoff, prioritized backlog, estimates, Definition of Done, release/milestone map), continues through execution and QA, and ends with close and retrospective. Key artifacts (one‑pager, roadmap/release plan, sprint backlog, acceptance criteria, risk register, and retrospectives) are tracked in the repo as the source of truth.

Core project workflows emphasize predictable delivery and quality. Teams use a project board (Backlog → Ready → In Progress → In Review → QA → Done), keep PRs small with clear acceptance criteria, require CI tests and approvals, and follow staged, checklist-driven release/deployment (including incident handling and rollbacks). Blocker escalation moves from team → PM → Product Lead → Sponsor (plus special security protocols).

Personas and responsibilities are clearly defined: Product Managers (outcomes, prioritization), Project Managers (delivery and risk), Developers (implementation and testing), QA (validation), and Stakeholders (initial inputs/approvals). Communications use daily standups, weekly syncs, sprint demos, and monthly updates. QA is integrated with automated and manual testing, security scanning, and CI gates; retrospectives produce actionable improvements for future work.

---

## Documentation Index

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

---

## How to Use

- Treat the docs in this folder as your reference for running projects at OctoAcme.
- Use the provided templates, checklists, and playbooks as the basis for planning, releases, and retrospectives.
- To propose improvements or updates, see the issue template in `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml`.
- Add project-specific process artifacts to `.copilot/` if you want Copilot Spaces to use them as context.

---

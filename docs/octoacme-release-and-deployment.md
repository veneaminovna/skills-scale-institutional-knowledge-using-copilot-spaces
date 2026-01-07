# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability. The **Release Manager** coordinates all release activities and ensures this guide is followed. For detailed role responsibilities, see [Roles & Personas](./octoacme-roles-and-personas.md).

## Release Manager Responsibilities
Release Managers use the [Release Manager Checklist](./release-manager-checklist.md) to coordinate releases, manage deployment processes, and communicate with stakeholders throughout the release lifecycle.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

---

## Related Documentation

- [Release Manager Checklist](./release-manager-checklist.md) - Comprehensive release management guide
- [Roles & Personas](./octoacme-roles-and-personas.md) - Release Manager role definition
- [Risk Management & Communication](./octoacme-risks-and-communication.md) - Risk management processes
- [Project Management Overview](./octoacme-project-management-overview.md) - Overall process context


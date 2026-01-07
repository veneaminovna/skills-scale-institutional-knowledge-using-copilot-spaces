# Release Manager Checklist

This comprehensive checklist guides Release Managers through the complete release lifecycle from planning through post-deployment. Use this checklist for every release to ensure consistency and reduce deployment risks.

## Pre-Planning Phase

### Release Scope Definition
- [ ] Review upcoming features and fixes planned for release
- [ ] Confirm release type (Patch / Minor / Major)
- [ ] Identify release version number following semantic versioning
- [ ] Review dependencies on other teams or systems
- [ ] Confirm release aligns with product roadmap

### Stakeholder Coordination
- [ ] Schedule release planning meeting with Product Manager and Project Manager
- [ ] Identify all stakeholders who need release notifications
- [ ] Confirm release timing with business stakeholders
- [ ] Verify no conflicting releases or blackout periods
- [ ] Document stakeholder communication plan

---

## Planning Phase (2-4 Weeks Before Release)

### Release Preparation
- [ ] Create release branch or tag in version control
- [ ] Document release timeline with key milestones
- [ ] Schedule deployment window (if required)
- [ ] Identify release cut-off date for feature freeze
- [ ] Schedule go/no-go meeting 24 hours before deployment

### Team Coordination
- [ ] Brief developers on release timeline and expectations
- [ ] Coordinate with QA on testing requirements and schedule
- [ ] Engage Technical Architect for architecture review
- [ ] Notify Risk & Compliance Lead of upcoming release
- [ ] Coordinate with Change Manager for change approvals

### Environment Preparation
- [ ] Verify staging environment is ready
- [ ] Confirm production environment capacity and readiness
- [ ] Review infrastructure changes or prerequisites
- [ ] Verify backup and rollback procedures are tested
- [ ] Confirm monitoring and alerting are configured

### Documentation
- [ ] Start draft of release notes
- [ ] Document migration steps (if any)
- [ ] Create deployment runbook
- [ ] Document rollback procedure
- [ ] Prepare smoke test checklist

---

## Pre-Release Phase (1 Week Before Release)

### Quality Verification
- [ ] Verify all PRs are merged and tagged for release
- [ ] Confirm all acceptance criteria are met
- [ ] Review CI/CD pipeline status (all checks passing)
- [ ] Confirm code review and approval requirements met
- [ ] Verify security scans are clean or issues triaged

### Testing Validation
- [ ] Confirm unit tests passing
- [ ] Confirm integration tests passing
- [ ] Review manual QA test results
- [ ] Verify performance test results (if applicable)
- [ ] Confirm accessibility testing completed (if applicable)

### Release Artifacts
- [ ] Build release candidate
- [ ] Verify build artifacts and checksums
- [ ] Tag release in version control
- [ ] Upload artifacts to release repository
- [ ] Document known issues and workarounds

### Risk Assessment
- [ ] Review risk register with Risk & Compliance Lead
- [ ] Confirm compliance requirements are met
- [ ] Document high-risk areas and monitoring plans
- [ ] Confirm rollback plan is tested and documented
- [ ] Verify on-call coverage during and after deployment

---

## Staging Deployment (2-3 Days Before Production)

### Staging Deployment
- [ ] Deploy release to staging environment
- [ ] Run automated smoke tests
- [ ] Execute manual smoke test checklist
- [ ] Verify database migrations (if applicable)
- [ ] Confirm integrations with external systems
- [ ] Monitor staging environment for issues

### Final Preparations
- [ ] Finalize release notes
- [ ] Update deployment runbook with any changes
- [ ] Prepare communication templates for stakeholders
- [ ] Schedule announcement timing
- [ ] Confirm support team is briefed on changes

### Go/No-Go Decision
- [ ] Conduct go/no-go meeting with stakeholders
- [ ] Review all quality gates and acceptance criteria
- [ ] Confirm no blocking issues or critical risks
- [ ] Document go/no-go decision and participants
- [ ] Communicate final deployment plan

---

## Production Deployment Day

### Pre-Deployment
- [ ] Verify deployment window is clear
- [ ] Confirm all stakeholders are notified
- [ ] Verify backup is created (if applicable)
- [ ] Confirm on-call team is available
- [ ] Start incident channel for coordination

### Deployment Execution
- [ ] Execute deployment according to runbook
- [ ] Monitor deployment progress and logs
- [ ] Verify database migrations completed successfully
- [ ] Confirm services are starting correctly
- [ ] Document any deviations from planned procedure

### Post-Deployment Verification
- [ ] Run automated smoke tests in production
- [ ] Execute manual verification checklist
- [ ] Monitor application logs for errors
- [ ] Check performance metrics and dashboards
- [ ] Verify integrations with external systems
- [ ] Confirm user authentication and authorization

### Communication
- [ ] Post deployment status in incident channel
- [ ] Notify stakeholders of successful deployment
- [ ] Announce release to support team
- [ ] Update status page (if applicable)
- [ ] Send release notes to customers/users

---

## Post-Deployment Monitoring (24-48 Hours)

### Active Monitoring
- [ ] Monitor error rates and application health
- [ ] Review customer support tickets for issues
- [ ] Track performance metrics vs. baseline
- [ ] Monitor user feedback channels
- [ ] Watch for unusual patterns or anomalies

### Stakeholder Updates
- [ ] Send 4-hour post-deployment status update
- [ ] Send 24-hour post-deployment summary
- [ ] Report any incidents or issues identified
- [ ] Communicate resolution of any post-deployment issues

---

## Rollback Procedure (If Needed)

### Rollback Decision
- [ ] Identify critical issue requiring rollback
- [ ] Notify incident response team immediately
- [ ] Brief stakeholders on rollback decision
- [ ] Document issue and rollback trigger

### Rollback Execution
- [ ] Execute rollback procedure from runbook
- [ ] Verify services return to previous state
- [ ] Confirm rollback is successful
- [ ] Monitor for additional issues
- [ ] Communicate rollback completion to stakeholders

### Post-Rollback
- [ ] Conduct immediate incident debrief
- [ ] Document root cause (preliminary)
- [ ] Create action items for fix
- [ ] Schedule blameless post-mortem
- [ ] Update release plan for next attempt

---

## Post-Release Activities (Within 1 Week)

### Release Closure
- [ ] Archive release artifacts and documentation
- [ ] Update version numbers for next release
- [ ] Close release tracking issues
- [ ] Archive incident channel
- [ ] Document lessons learned

### Retrospective
- [ ] Schedule release retrospective with team
- [ ] Collect feedback from stakeholders
- [ ] Identify process improvements
- [ ] Update release checklist based on learnings
- [ ] Share key takeaways with broader organization

### Metrics & Reporting
- [ ] Track deployment time and duration
- [ ] Measure deployment success rate
- [ ] Report on issues found post-deployment
- [ ] Calculate MTTR for any incidents
- [ ] Update release metrics dashboard

---

## Emergency/Hotfix Release

For critical production issues requiring immediate release:

- [ ] Declare incident and notify leadership
- [ ] Create hotfix branch from production
- [ ] Implement minimal fix to address critical issue
- [ ] Fast-track code review (minimum 1 reviewer)
- [ ] Run essential tests only (smoke tests + regression for affected area)
- [ ] Brief Risk & Compliance Lead on emergency release
- [ ] Deploy to staging and verify fix
- [ ] Get emergency approval from Product Lead
- [ ] Deploy to production with elevated monitoring
- [ ] Communicate broadly about hotfix and impact
- [ ] Schedule retrospective within 48 hours

---

## Release Types Reference

### Patch Release (x.x.X)
- Hotfixes for critical bugs
- Security patches
- Minor documentation fixes
- **Timeline:** Can be expedited (same day to 1 week)
- **Checklist:** Use abbreviated checklist focusing on critical items

### Minor Release (x.X.0)
- New features (backward compatible)
- Performance improvements
- Non-breaking changes
- **Timeline:** 2-4 weeks planning and preparation
- **Checklist:** Use full checklist

### Major Release (X.0.0)
- Breaking changes
- Major new features
- Architecture changes
- **Timeline:** 4-8 weeks planning and preparation
- **Checklist:** Use full checklist + additional architecture review

---

## Related Documentation

- [Release & Deployment Guide](./octoacme-release-and-deployment.md) - Release process overview
- [Roles & Personas](./octoacme-roles-and-personas.md) - Release Manager role definition
- [Risk Escalation Path Template](./risk-escalation-path-template.md) - Escalation procedures
- [Risk Management & Communication](./octoacme-risks-and-communication.md) - Risk management processes

---

## Customization Notes

- Adjust timeline and checklist items based on release complexity
- Add organization-specific compliance or regulatory requirements
- Include any custom tooling or automation steps
- Update based on lessons learned from retrospectives

---

*This checklist supports the Release Manager role defined in issue #5 and integrates with existing OctoAcme process documentation.*

# Risk Escalation Path Template

This template provides a structured approach for escalating risks based on severity, impact, and urgency. Use this guide to ensure timely communication and appropriate decision-making authority at each escalation level.

## Risk Escalation Levels

### Level 1: Team-Level Risk
**When to use:** Low impact risks that can be resolved within the team

**Responsible Parties:**
- Team Lead or Senior Developer
- Scrum Master (if applicable)

**Decision Authority:**
- Team can implement mitigation without external approval

**Response Time:**
- Identify and address within current sprint
- Review in daily standup

**Communication:**
- Document in team's risk log
- Discuss in daily standup or team meeting
- Update project board with mitigation tasks

**Escalation Trigger:**
- Risk remains unresolved after 1 sprint
- Impact increases to medium or high
- Team lacks authority or resources to mitigate

---

### Level 2: Project Manager & Risk Lead
**When to use:** Medium impact risks or unresolved Level 1 risks

**Responsible Parties:**
- Project Manager
- Risk & Compliance Lead

**Decision Authority:**
- Can adjust project scope, timelines, or resource allocation
- Can engage additional teams or stakeholders

**Response Time:**
- Acknowledge within 1 business day
- Action plan created within 2 business days
- Weekly review in PM sync meetings

**Communication:**
- Add to project risk register with status updates
- Include in weekly status reports
- Brief Product Manager and Technical Architect
- Update stakeholders if timeline or scope is impacted

**Escalation Trigger:**
- Risk cannot be mitigated within project authority
- High likelihood of schedule or budget impact
- Multiple teams or external dependencies involved
- Compliance or security concerns identified

---

### Level 3: Product Lead & Program Manager
**When to use:** High impact risks affecting multiple projects or strategic objectives

**Responsible Parties:**
- Product Lead
- Program Manager
- Risk & Compliance Lead

**Decision Authority:**
- Can reprioritize roadmap and reallocate resources across projects
- Can approve budget increases or timeline extensions
- Can engage executive leadership for support

**Response Time:**
- Acknowledge immediately (within 4 hours)
- Emergency meeting scheduled within 24 hours
- Mitigation plan approved within 48 hours

**Communication:**
- Immediate notification via email and direct message
- Present risk assessment with data and options
- Schedule emergency planning meeting
- Document decisions and communicate to all affected teams
- Provide status updates to sponsors daily until resolved

**Escalation Trigger:**
- Risk threatens project success or organizational reputation
- Financial impact exceeds program budget authority
- Legal, regulatory, or security incident
- Requires executive decision-making

---

### Level 4: Executive Sponsor & Leadership
**When to use:** Critical risks with organization-wide impact

**Responsible Parties:**
- Executive Sponsor
- VP/C-Level Leadership
- Risk & Compliance Lead

**Decision Authority:**
- Final authority on strategic decisions
- Can halt or pivot projects
- Can approve significant financial commitments

**Response Time:**
- Immediate escalation (within 1 hour)
- Executive briefing within 2 hours
- Decision and action plan within 4-8 hours

**Communication:**
- Direct escalation to executive sponsor
- Executive briefing with risk assessment and recommendations
- Crisis communication plan activated if needed
- Board notification if required by governance policies
- Company-wide communication if appropriate

---

## Risk Escalation Template

Use this template when escalating a risk:

```markdown
## Risk Escalation: [Brief Risk Title]

**Date:** [Date]
**Reported By:** [Name, Role]
**Current Escalation Level:** [1, 2, 3, or 4]

### Risk Summary
[Brief description of the risk in 2-3 sentences]

### Impact Assessment
- **Severity:** [Critical / High / Medium / Low]
- **Likelihood:** [Very High / High / Medium / Low]
- **Impact Areas:** [Schedule / Budget / Quality / Compliance / Security]
- **Affected Projects/Teams:** [List]

### Current Status
- **When Identified:** [Date]
- **Current Mitigation Efforts:** [What has been tried]
- **Why Escalating:** [What changed or why current approach is insufficient]

### Requested Action
[Specific decisions or resources needed to mitigate the risk]

### Options Analysis
1. **Option 1:** [Description, pros, cons, estimated impact]
2. **Option 2:** [Description, pros, cons, estimated impact]
3. **Option 3 (if applicable):** [Description, pros, cons, estimated impact]

### Recommendation
[Your recommended approach with justification]

### Timeline Implications
- **If resolved by [date]:** [Impact]
- **If delayed beyond [date]:** [Impact]

### Supporting Information
- Links to risk register entry
- Related incidents or issues
- Supporting data or metrics
```

---

## Risk Assessment Criteria

Use these criteria to determine escalation level:

| Factor | Level 1 (Low) | Level 2 (Medium) | Level 3 (High) | Level 4 (Critical) |
|--------|---------------|------------------|----------------|--------------------|
| **Schedule Impact** | < 1 week | 1-2 weeks | 2-4 weeks | > 4 weeks or milestone miss |
| **Budget Impact** | < $5K | $5K-$25K | $25K-$100K | > $100K |
| **Team Impact** | Single team | 2-3 teams | Multiple teams | Organization-wide |
| **Customer Impact** | None | Low (minor inconvenience) | Medium (affects workflow) | High (critical failure) |
| **Reputation Risk** | None | Minimal | Moderate | Severe |
| **Compliance/Legal** | None | Minor concern | Compliance issue | Legal/regulatory violation |

---

## Best Practices

1. **Escalate Early:** Don't wait until a risk becomes a crisis
2. **Be Specific:** Provide concrete data and clear impact assessment
3. **Offer Options:** Present multiple solutions with pros and cons
4. **Follow Up:** Update stakeholders on progress and resolution
5. **Document Everything:** Maintain clear audit trail of decisions
6. **Learn:** Capture lessons learned for future risk management

---

## Related Documentation

- [Risk Management & Communication](./octoacme-risks-and-communication.md) - Risk management processes
- [Roles & Personas](./octoacme-roles-and-personas.md) - Risk & Compliance Lead role details
- [Project Management Overview](./octoacme-project-management-overview.md) - Overall process context

---

*This template supports the expanded roles defined in issue #5 and provides clear escalation paths for the Risk & Compliance Lead, Project Managers, and other stakeholders.*

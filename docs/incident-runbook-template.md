# Incident Runbook Template

This template provides a structured approach for incident coordination, communication, and resolution.

> **Related docs**: [Roles & Personas](octoacme-roles-and-personas.md) | [Risk Management & Communication](octoacme-risks-and-communication.md) | [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

---

## Incident Overview

| Field | Value |
|-------|-------|
| Incident ID | |
| Incident Title | |
| Severity | |
| Status | Open / Investigating / Mitigating / Resolved / Closed |
| Start Time | |
| Detection Time | |
| Resolution Time | |
| Duration | |

---

## Severity Definition

| Severity | Description | Examples | Response Time |
|----------|-------------|----------|---------------|
| **SEV-1 (Critical)** | Complete service outage or data loss affecting all users | Production down, data breach, complete loss of service | Immediate (< 15 min) |
| **SEV-2 (High)** | Major functionality impaired or significant user impact | Key feature unavailable, significant performance degradation | < 30 minutes |
| **SEV-3 (Medium)** | Limited functionality impact or minor user impact | Non-critical feature issues, intermittent problems | < 2 hours |
| **SEV-4 (Low)** | Minimal impact, cosmetic issues, or workaround available | UI issues, minor bugs with workarounds | Next business day |

---

## Incident Roles

| Role | Assigned To | Contact |
|------|-------------|---------|
| **Incident Commander** | | |
| **Communications Lead** | | |
| **Technical Lead** | | |
| **Scribe** | | |

### Role Responsibilities

#### Incident Commander
- Overall coordination of incident response
- Makes decisions on escalation and mitigation
- Delegates tasks to team members
- Declares incident resolved/closed

#### Communications Lead
- Manages internal and external communications
- Provides status updates to stakeholders
- Coordinates with support and customer success
- Drafts incident notifications

#### Technical Lead
- Leads technical investigation and mitigation
- Coordinates with engineering teams
- Implements fixes and workarounds
- Verifies resolution

#### Scribe
- Documents timeline and actions
- Records decisions and rationale
- Captures action items
- Prepares incident report

---

## Communication Plan

### Internal Communication

| Audience | Channel | Frequency | Owner |
|----------|---------|-----------|-------|
| Engineering Team | Slack #incidents | Real-time | Communications Lead |
| Leadership | Email / Slack | Every 30 min (SEV-1/2) | Communications Lead |
| Support Team | Slack #support | Real-time | Communications Lead |
| On-call Team | PagerDuty | Immediate | Incident Commander |

### External Communication (if applicable)

| Audience | Channel | Frequency | Owner |
|----------|---------|-----------|-------|
| Customers | Status Page | As needed | Communications Lead |
| Partners | Email | As needed | Communications Lead |

### Status Update Template

```
**Incident Update - [Incident Title]**

Status: [Investigating/Mitigating/Resolved]
Severity: [SEV-1/2/3/4]
Time: [Current Time]

**Current Status:**
[Brief description of current situation]

**Impact:**
[Description of user/system impact]

**Actions Taken:**
[List of actions taken since last update]

**Next Steps:**
[Planned actions]

**ETA:**
[Estimated time to resolution, if known]

---
Next update in [X] minutes.
```

---

## Incident Timeline

| Time | Event | Action Taken | Owner |
|------|-------|--------------|-------|
| | Incident detected | | |
| | Initial assessment | | |
| | Escalation (if applicable) | | |
| | Mitigation started | | |
| | Status update sent | | |
| | Resolution verified | | |
| | Incident closed | | |

---

## Mitigation Steps

### Initial Triage
- [ ] Confirm the incident is real (not a false alarm)
- [ ] Assess severity and impact
- [ ] Assign incident roles
- [ ] Begin documentation

### Investigation
- [ ] Review monitoring dashboards
- [ ] Check recent changes/deployments
- [ ] Examine logs and error messages
- [ ] Identify affected systems/services
- [ ] Determine root cause hypothesis

### Mitigation Options

| Option | Description | Pros | Cons | Risk Level |
|--------|-------------|------|------|------------|
| Rollback | Revert to previous version | Quick | May lose features | Low |
| Hotfix | Deploy targeted fix | Addresses issue | Needs testing | Medium |
| Workaround | Temporary solution | Fast | Not permanent | Low |
| Scale | Add resources | May resolve load issues | Cost | Low |

### Mitigation Execution
- [ ] Mitigation option selected and approved
- [ ] Change implemented
- [ ] Verification performed
- [ ] Stakeholders notified

---

## Resolution Verification

### Verification Checklist
- [ ] Service health restored
- [ ] Key user flows working
- [ ] Error rates back to normal
- [ ] Performance metrics stable
- [ ] No new errors in logs
- [ ] Monitoring alerts cleared

### Sign-off

| Role | Name | Verified | Time |
|------|------|----------|------|
| Technical Lead | | ☐ | |
| Incident Commander | | ☐ | |

---

## Post-Incident Review Checklist

### Scheduling
- [ ] Post-incident review scheduled within 48-72 hours
- [ ] All participants invited
- [ ] Incident timeline prepared
- [ ] Data and logs preserved

### Review Agenda
1. Incident summary and timeline review
2. What went well
3. What could be improved
4. Root cause analysis
5. Action items and owners
6. Process improvements

### Action Items Template

| ID | Action Item | Owner | Priority | Due Date | Status |
|----|-------------|-------|----------|----------|--------|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |

### Root Cause Analysis

**What happened?**
_Describe the incident in detail._

**Why did it happen?**
_Use 5 Whys or similar technique._

**How was it detected?**
_Monitoring, user report, etc._

**How was it resolved?**
_Describe the fix/mitigation._

**How can we prevent it?**
_Preventive measures._

---

## Post-Incident Report Template

### Executive Summary
_Brief summary of the incident for leadership._

### Impact
- **Users Affected**: 
- **Duration**: 
- **Revenue Impact** (if applicable): 
- **SLA Impact** (if applicable): 

### Timeline
_Key events with timestamps._

### Root Cause
_Clear explanation of what caused the incident._

### Resolution
_How the incident was resolved._

### Action Items
_List of follow-up actions with owners and due dates._

### Lessons Learned
_Key takeaways for the team._

---

## Appendix

### Escalation Contacts

| Role | Primary Contact | Backup Contact |
|------|-----------------|----------------|
| Engineering On-call | | |
| DevOps On-call | | |
| Security On-call | | |
| Management | | |

### Useful Links
- Monitoring Dashboard: 
- Log Aggregator: 
- Runbook Library: 
- Status Page Admin: 

### Related Runbooks
- Database Failover Runbook
- CDN Failover Runbook
- Authentication Service Runbook
- Payment System Runbook

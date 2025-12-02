# Personas Interaction Matrix

This matrix maps new personas to existing roles and typical touchpoints across project phases.

> **Related docs**: [Roles & Personas](octoacme-roles-and-personas.md) | [Project Management Overview](octoacme-project-management-overview.md)

---

## Overview

This document provides a quick reference for understanding how new personas interact with existing roles and when they are typically involved in project activities.

### Existing Core Roles
- **Product Owner (PO)**: Defines outcomes, prioritizes backlog
- **Engineering Lead (EL)**: Technical leadership and implementation
- **Project Manager (PM)**: Coordinates delivery, schedules, risk
- **DevOps**: Infrastructure, CI/CD, deployment
- **QA**: Quality verification and testing
- **Stakeholders**: Business alignment and approvals

### New Personas
- Release Coordinator
- QA Lead (Test Owner)
- Security Liaison (Security Champion)
- Vendor / Contract Manager
- Accessibility Advocate
- Data Analyst (Metrics Owner)
- Technical Writer / Documentation Owner
- On-call Incident Coordinator

---

## Interaction Matrix

### Legend
- ●● = Primary interaction (frequent, close collaboration)
- ● = Secondary interaction (regular touchpoint)
- ○ = Occasional interaction (as needed)
- — = Minimal/no direct interaction

| New Persona | Product Owner | Engineering Lead | Project Manager | DevOps | QA | Stakeholders |
|-------------|:-------------:|:----------------:|:---------------:|:------:|:--:|:------------:|
| **Release Coordinator** | ●● | ●● | ●● | ●● | ●● | ●● |
| **QA Lead (Test Owner)** | ●● | ●● | ● | ● | ●● | ○ |
| **Security Liaison** | ● | ●● | ● | ●● | ● | ○ |
| **Vendor / Contract Manager** | ● | ● | ●● | ○ | ○ | ● |
| **Accessibility Advocate** | ●● | ●● | ● | ○ | ●● | ● |
| **Data Analyst** | ●● | ● | ● | ● | ● | ●● |
| **Technical Writer** | ●● | ●● | ● | ● | ● | ● |
| **On-call Incident Coordinator** | ● | ●● | ● | ●● | ● | ●● |

---

## Process Phase Involvement

### Legend
- ✓✓ = Primary responsibility / heavily involved
- ✓ = Participates / contributes
- ○ = Consulted as needed
- — = Not typically involved

| New Persona | Planning | Execution | Release | Incident | Retrospective |
|-------------|:--------:|:---------:|:-------:|:--------:|:-------------:|
| **Release Coordinator** | ✓ | ○ | ✓✓ | ✓ | ✓ |
| **QA Lead (Test Owner)** | ✓✓ | ✓✓ | ✓✓ | ✓ | ✓ |
| **Security Liaison** | ✓ | ✓ | ✓ | ✓✓ | ✓ |
| **Vendor / Contract Manager** | ✓✓ | ✓ | ✓ | ○ | ✓ |
| **Accessibility Advocate** | ✓✓ | ✓ | ✓ | ○ | ✓ |
| **Data Analyst** | ✓ | ○ | ✓ | ✓ | ✓✓ |
| **Technical Writer** | ✓ | ✓ | ✓✓ | ✓ | ○ |
| **On-call Incident Coordinator** | ✓ | ○ | ✓ | ✓✓ | ✓✓ |

---

## Detailed Touchpoints by Phase

### Planning Phase

| Persona | Typical Activities | Key Collaborators |
|---------|-------------------|-------------------|
| **Release Coordinator** | Define release schedule, identify dependencies | PM, PO, EL |
| **QA Lead** | Define test strategy, acceptance criteria | PO, EL, QA |
| **Security Liaison** | Identify security requirements, threat modeling | EL, DevOps |
| **Vendor / Contract Manager** | Include vendor timelines, coordinate deliverables | PM, PO, Finance |
| **Accessibility Advocate** | Define accessibility requirements | PO, EL, QA |
| **Data Analyst** | Define success metrics, instrumentation plan | PO, EL |
| **Technical Writer** | Identify documentation requirements | PO, EL, PM |
| **On-call Incident Coordinator** | Define incident response procedures | DevOps, EL, PM |

### Execution Phase

| Persona | Typical Activities | Key Collaborators |
|---------|-------------------|-------------------|
| **Release Coordinator** | Monitor progress, coordinate release prep | PM, EL, QA |
| **QA Lead** | Execute testing, track quality metrics | QA, EL, Developers |
| **Security Liaison** | Security reviews, vulnerability tracking | EL, DevOps |
| **Vendor / Contract Manager** | Track vendor deliverables, manage issues | PM, Vendors |
| **Accessibility Advocate** | Accessibility reviews, testing | QA, EL, Developers |
| **Data Analyst** | Set up dashboards, monitor metrics | EL, DevOps |
| **Technical Writer** | Create/update documentation | EL, PO, Developers |
| **On-call Incident Coordinator** | Monitor systems, respond to issues | DevOps, EL |

### Release Phase

| Persona | Typical Activities | Key Collaborators |
|---------|-------------------|-------------------|
| **Release Coordinator** | Lead release execution, coordinate teams | All roles |
| **QA Lead** | QA sign-off, final verification | QA, Release Coord |
| **Security Liaison** | Security verification, compliance check | DevOps, EL |
| **Vendor / Contract Manager** | Coordinate vendor components | PM, Vendors, EL |
| **Accessibility Advocate** | Accessibility verification | QA, PO |
| **Data Analyst** | Monitor release metrics | DevOps, EL |
| **Technical Writer** | Finalize release documentation | PO, Release Coord |
| **On-call Incident Coordinator** | Standby for release issues | DevOps, EL |

### Incident Phase

| Persona | Typical Activities | Key Collaborators |
|---------|-------------------|-------------------|
| **Release Coordinator** | Coordinate rollback if needed | DevOps, EL, Incident Coord |
| **QA Lead** | Assist with root cause, test fixes | EL, Developers |
| **Security Liaison** | Lead security incidents, coordinate response | EL, DevOps, Incident Coord |
| **Vendor / Contract Manager** | Escalate vendor-related issues | PM, Vendors |
| **Accessibility Advocate** | Address accessibility incidents | QA, EL |
| **Data Analyst** | Provide data analysis, impact assessment | EL, Incident Coord |
| **Technical Writer** | Document incident, update runbooks | Incident Coord, EL |
| **On-call Incident Coordinator** | Lead incident response, coordinate resolution | All roles |

### Retrospective Phase

| Persona | Typical Activities | Key Collaborators |
|---------|-------------------|-------------------|
| **Release Coordinator** | Share release learnings, process improvements | PM, Team |
| **QA Lead** | Share quality insights, propose improvements | QA, Team |
| **Security Liaison** | Share security learnings, update practices | Team |
| **Vendor / Contract Manager** | Review vendor performance | PM, Stakeholders |
| **Accessibility Advocate** | Share accessibility insights | Team |
| **Data Analyst** | Present metrics, outcomes analysis | PO, PM, Stakeholders |
| **Technical Writer** | Capture documentation improvements | Team |
| **On-call Incident Coordinator** | Lead post-incident review, action items | Team |

---

## Communication Channels

| Persona | Primary Channels | Escalation Path |
|---------|-----------------|-----------------|
| **Release Coordinator** | Release channel, team standups | PM → EL → Sponsor |
| **QA Lead** | QA channel, team standups | PM → PO |
| **Security Liaison** | Security channel, team standups | PM → Security Team |
| **Vendor / Contract Manager** | Vendor meetings, PM syncs | PM → Finance → Legal |
| **Accessibility Advocate** | Team channel, design reviews | PM → PO |
| **Data Analyst** | Analytics channel, stakeholder reports | PM → PO |
| **Technical Writer** | Docs channel, team reviews | PM → PO |
| **On-call Incident Coordinator** | Incident channel, PagerDuty | Incident → EL → Management |

---

## Quick Reference: Who to Contact

| I need help with... | Contact |
|--------------------|---------|
| Release scheduling and coordination | Release Coordinator |
| Test strategy and QA sign-off | QA Lead |
| Security concerns and compliance | Security Liaison |
| Vendor deliverables and contracts | Vendor / Contract Manager |
| Accessibility requirements | Accessibility Advocate |
| Metrics and data analysis | Data Analyst |
| Documentation needs | Technical Writer |
| Production incidents | On-call Incident Coordinator |

---

## Supporting Documents

- [Release Coordinator Checklist](release-coordinator-checklist.md)
- [QA Release Checklist](qa-release-checklist.md)
- [Incident Runbook Template](incident-runbook-template.md)
- [Vendor Management Guidelines](vendor-management-guidelines.md)

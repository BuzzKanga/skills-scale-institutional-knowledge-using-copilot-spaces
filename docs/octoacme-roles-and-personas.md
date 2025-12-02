# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

## Supporting Documents

The following documents provide additional templates and checklists for specific roles:

- [Release Coordinator Checklist](release-coordinator-checklist.md)
- [QA Release Checklist](qa-release-checklist.md)
- [Incident Runbook Template](incident-runbook-template.md)
- [Vendor Management Guidelines](vendor-management-guidelines.md)
- [Personas Interaction Matrix](personas-interaction-matrix.md)

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

## Release Coordinator

### Role Summary
The Release Coordinator (or Release Manager) oversees release planning and execution, coordinating between development, operations, and QA teams to ensure production readiness. They manage the release schedule, track dependencies, and communicate release status to stakeholders.

### Responsibilities
- Own the release schedule and communicate release windows to stakeholders
- Coordinate code freeze, CI verification, and dependency checks
- Ensure rollback plans and monitoring are in place before deployment
- Manage stakeholder notifications and release documentation
- Conduct post-release validation and capture lessons learned

### Key Interactions
- **Product Owner**: Align on feature priorities and release scope
- **Engineering Lead**: Coordinate code freeze and technical readiness
- **Project Manager**: Communicate release timelines and dependencies
- **DevOps**: Coordinate deployment pipelines and infrastructure readiness
- **QA**: Ensure test completion and sign-off before release
- **Stakeholders**: Provide release status updates and announcements

### Process Involvement
- **Planning**: Participate in release planning and milestone setting
- **Release**: Lead release execution using the [Release Coordinator Checklist](release-coordinator-checklist.md)
- **Incident**: Coordinate with On-call Incident Coordinator for release-related incidents
- **Retrospective**: Capture release process improvements

---

## QA Lead (Test Owner)

### Role Summary
The QA Lead defines the test strategy, ensures quality gates are established and met, and coordinates testing activities across the team. They own the overall test coverage and sign-off for releases.

### Responsibilities
- Define and maintain the test strategy and automation framework
- Establish quality gates and acceptance criteria for releases
- Coordinate regression, smoke, and acceptance testing
- Review test coverage and identify gaps
- Provide final QA sign-off for releases

### Key Interactions
- **Product Owner**: Clarify acceptance criteria and user stories
- **Engineering Lead**: Align on testability and technical implementation
- **Project Manager**: Report testing status and blockers
- **DevOps**: Ensure CI/CD pipelines include proper test stages
- **QA Team**: Coordinate testing activities and resources
- **Stakeholders**: Communicate quality status and risks

### Process Involvement
- **Planning**: Define test approach and acceptance criteria
- **Release**: Execute QA sign-off using the [QA Release Checklist](qa-release-checklist.md)
- **Incident**: Assist with root cause analysis and test gap identification
- **Retrospective**: Propose quality and process improvements

---

## Security Liaison (Security Champion)

### Role Summary
The Security Liaison acts as the security advocate within the team, ensuring security best practices are followed throughout the development lifecycle. They bridge the gap between the security team and the delivery team.

### Responsibilities
- Advocate for security best practices in design and code reviews
- Coordinate security scanning and vulnerability remediation
- Escalate security risks to the Security team and Project Manager
- Ensure compliance with security policies and standards
- Support incident response for security-related incidents

### Key Interactions
- **Product Owner**: Advise on security implications of features
- **Engineering Lead**: Review security aspects of technical designs
- **Project Manager**: Report security risks and remediation status
- **DevOps**: Ensure security scanning is integrated in CI/CD
- **QA**: Coordinate security testing activities
- **Stakeholders**: Communicate security posture and compliance status

### Process Involvement
- **Planning**: Identify security requirements and risks
- **Release**: Verify security scans pass before deployment
- **Incident**: Lead security incident response and coordination
- **Retrospective**: Capture security lessons learned

---

## Vendor / Contract Manager

### Role Summary
The Vendor / Contract Manager maintains relationships with external vendors and contractors, ensuring deliverables are tracked, timelines are met, and contracts are managed effectively.

### Responsibilities
- Own vendor relationships and contract timelines
- Track vendor deliverables and milestones
- Escalate vendor issues to Project Manager and Finance
- Coordinate vendor onboarding and offboarding
- Maintain vendor documentation and compliance records

### Key Interactions
- **Product Owner**: Align vendor deliverables with product requirements
- **Engineering Lead**: Coordinate technical integration with vendors
- **Project Manager**: Report vendor status and escalate issues
- **DevOps**: Coordinate vendor access and integration points
- **QA**: Ensure vendor deliverables meet quality standards
- **Stakeholders**: Communicate vendor performance and risks

### Process Involvement
- **Planning**: Include vendor timelines in project planning
- **Release**: Coordinate vendor components for release
- **Incident**: Escalate vendor-related incidents
- **Retrospective**: Review vendor performance and relationship

See [Vendor Management Guidelines](vendor-management-guidelines.md) for detailed processes.

---

## Accessibility Advocate

### Role Summary
The Accessibility Advocate ensures products are accessible to all users, including those with disabilities. They promote accessibility best practices and coordinate compliance with accessibility standards (e.g., WCAG).

### Responsibilities
- Advocate for accessibility in design and development
- Review features for accessibility compliance
- Coordinate accessibility testing and audits
- Educate the team on accessibility best practices
- Track and prioritize accessibility issues

### Key Interactions
- **Product Owner**: Advise on accessibility requirements for features
- **Engineering Lead**: Guide accessible implementation patterns
- **Project Manager**: Report accessibility status and blockers
- **DevOps**: Ensure accessibility tools are available in CI/CD
- **QA**: Coordinate accessibility testing
- **Stakeholders**: Communicate accessibility compliance status

### Process Involvement
- **Planning**: Define accessibility requirements and acceptance criteria
- **Release**: Verify accessibility compliance before release
- **Incident**: Assist with accessibility-related issues
- **Retrospective**: Propose accessibility improvements

---

## Data Analyst (Metrics Owner)

### Role Summary
The Data Analyst owns the definition, collection, and analysis of project and product metrics. They provide data-driven insights to support decision-making and measure outcomes.

### Responsibilities
- Define success metrics and KPIs for projects and features
- Set up dashboards and reporting for key metrics
- Analyze data to provide actionable insights
- Support A/B testing and experimentation
- Report on outcomes and trends to stakeholders

### Key Interactions
- **Product Owner**: Define and track product success metrics
- **Engineering Lead**: Coordinate instrumentation and data collection
- **Project Manager**: Provide project health metrics and reports
- **DevOps**: Ensure observability and logging are in place
- **QA**: Analyze quality metrics and trends
- **Stakeholders**: Present data insights and recommendations

### Process Involvement
- **Planning**: Define metrics and measurement approach
- **Release**: Monitor metrics during and after release
- **Incident**: Provide data analysis for incident investigation
- **Retrospective**: Present metrics and insights for discussion

---

## Technical Writer / Documentation Owner

### Role Summary
The Technical Writer owns the creation and maintenance of product and process documentation. They ensure documentation is accurate, accessible, and up-to-date.

### Responsibilities
- Create and maintain user-facing and internal documentation
- Coordinate documentation reviews and updates
- Ensure documentation aligns with product changes
- Maintain documentation standards and style guides
- Support knowledge sharing and onboarding

### Key Interactions
- **Product Owner**: Align documentation with product features
- **Engineering Lead**: Coordinate technical documentation
- **Project Manager**: Track documentation deliverables
- **DevOps**: Document deployment and operational procedures
- **QA**: Document testing procedures and results
- **Stakeholders**: Gather feedback on documentation needs

### Process Involvement
- **Planning**: Identify documentation requirements
- **Release**: Ensure documentation is ready for release
- **Incident**: Document incident response and learnings
- **Retrospective**: Capture process documentation improvements

---

## On-call Incident Coordinator

### Role Summary
The On-call Incident Coordinator manages incident response during production issues. They coordinate communication, triage, mitigation, and post-incident review.

### Responsibilities
- Serve as the incident commander during production incidents
- Coordinate communication with stakeholders and support
- Triage incidents and assign roles (communication, mitigation, etc.)
- Ensure incident timeline and actions are documented
- Facilitate post-incident review and action item tracking

### Key Interactions
- **Product Owner**: Communicate incident impact on product
- **Engineering Lead**: Coordinate technical mitigation and resolution
- **Project Manager**: Report incident status and impact
- **DevOps**: Coordinate infrastructure and deployment actions
- **QA**: Assist with incident testing and validation
- **Stakeholders**: Provide incident updates and resolution status

### Process Involvement
- **Planning**: Define incident response procedures
- **Release**: Coordinate with Release Coordinator for release incidents
- **Incident**: Lead incident response using the [Incident Runbook Template](incident-runbook-template.md)
- **Retrospective**: Facilitate post-incident review and action items



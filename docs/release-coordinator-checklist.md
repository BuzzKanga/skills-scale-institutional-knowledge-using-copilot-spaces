# Release Coordinator Checklist

This checklist provides a step-by-step guide for the Release Coordinator to ensure release readiness and smooth deployment.

> **Related docs**: [Roles & Personas](octoacme-roles-and-personas.md) | [Release & Deployment Guide](octoacme-release-and-deployment.md)

---

## Pre-Release Readiness

### Code Freeze
- [ ] Code freeze date communicated to the team
- [ ] All planned features and fixes merged to release branch
- [ ] No unapproved changes after code freeze
- [ ] Release branch created and protected

### CI/CD Status
- [ ] All CI pipelines passing on release branch
- [ ] Security scans completed with no critical issues
- [ ] Static analysis checks passing
- [ ] All required tests passing (unit, integration, e2e)

### Dependency Verification
- [ ] All dependencies up-to-date and verified
- [ ] No known vulnerabilities in dependencies
- [ ] Third-party integrations tested and confirmed
- [ ] Vendor deliverables received and validated (if applicable)

### Rollback Plan
- [ ] Rollback procedure documented and reviewed
- [ ] Previous stable version identified for rollback
- [ ] Rollback tested in staging environment
- [ ] Rollback communication plan prepared

---

## Stakeholder Notifications

### Pre-Release Communication
- [ ] Release scope and timeline shared with stakeholders
- [ ] Release notes drafted and reviewed
- [ ] Support team notified and prepared
- [ ] Customer-facing communications prepared (if applicable)

### Deployment Window
- [ ] Deployment window scheduled and communicated
- [ ] On-call team notified
- [ ] Maintenance window announced (if applicable)
- [ ] Escalation contacts confirmed

---

## Documentation

### Release Documentation
- [ ] Release notes finalized
- [ ] Changelog updated
- [ ] User documentation updated (if applicable)
- [ ] Internal runbooks updated
- [ ] Migration steps documented (if applicable)

### Technical Documentation
- [ ] API documentation updated (if applicable)
- [ ] Configuration changes documented
- [ ] Known issues documented
- [ ] Troubleshooting guide updated

---

## Monitoring & Observability

### Monitoring Setup
- [ ] Dashboards configured for release metrics
- [ ] Alerts configured for key indicators
- [ ] Log aggregation verified
- [ ] APM/tracing configured

### Success Criteria
- [ ] Success metrics defined (error rate, latency, etc.)
- [ ] Baseline metrics captured before release
- [ ] Thresholds for rollback decision documented

---

## Deployment Execution

### Staging Deployment
- [ ] Deployed to staging environment
- [ ] Smoke tests passed in staging
- [ ] QA sign-off received (see [QA Release Checklist](qa-release-checklist.md))
- [ ] Performance verified in staging

### Production Deployment
- [ ] Backup/snapshot taken (if applicable)
- [ ] Deployed to production
- [ ] Smoke tests passed in production
- [ ] Health checks verified
- [ ] Feature flags enabled/disabled as planned

---

## Post-Release Validation

### Immediate Validation (0-30 minutes)
- [ ] Application health verified
- [ ] Key user flows tested
- [ ] Error rates within acceptable thresholds
- [ ] No critical alerts triggered

### Extended Validation (30 minutes - 24 hours)
- [ ] Performance metrics stable
- [ ] User feedback monitored
- [ ] Support tickets reviewed
- [ ] Metrics trending as expected

### Communication
- [ ] Release announcement sent to stakeholders
- [ ] Support team confirmed ready
- [ ] Release complete notification sent

---

## Post-Release Activities

### Documentation
- [ ] Release retrospective scheduled
- [ ] Lessons learned captured
- [ ] Process improvements identified
- [ ] Runbooks updated with any new learnings

### Cleanup
- [ ] Feature flags cleaned up (if applicable)
- [ ] Temporary resources removed
- [ ] Release branch merged/archived

---

## Sign-off

| Role | Name | Sign-off Date |
|------|------|---------------|
| Release Coordinator | | |
| QA Lead | | |
| Engineering Lead | | |
| Product Owner | | |

---

## Notes

_Add any release-specific notes or exceptions here._

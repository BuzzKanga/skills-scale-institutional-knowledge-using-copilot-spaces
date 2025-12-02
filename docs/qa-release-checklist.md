# QA Release Checklist

This checklist provides QA acceptance criteria, testing procedures, and sign-off requirements for releases.

> **Related docs**: [Roles & Personas](octoacme-roles-and-personas.md) | [Release Coordinator Checklist](release-coordinator-checklist.md) | [Release & Deployment Guide](octoacme-release-and-deployment.md)

---

## Acceptance Criteria Template

### Feature: _[Feature Name]_

| Criterion | Expected Behavior | Verified | Notes |
|-----------|------------------|----------|-------|
| | | ☐ | |
| | | ☐ | |
| | | ☐ | |

### Acceptance Criteria Checklist
- [ ] All acceptance criteria clearly defined
- [ ] Edge cases identified and documented
- [ ] Error handling scenarios defined
- [ ] Accessibility requirements included
- [ ] Performance requirements specified

---

## Regression Test Checklist

### Core Functionality
- [ ] User authentication and authorization
- [ ] Key user workflows (list critical paths)
- [ ] Data integrity and persistence
- [ ] API endpoints and integrations
- [ ] Error handling and validation

### Cross-Browser/Platform Testing
- [ ] Chrome (latest version)
- [ ] Firefox (latest version)
- [ ] Safari (latest version)
- [ ] Edge (latest version)
- [ ] Mobile responsive testing

### Integration Points
- [ ] Third-party service integrations
- [ ] Database operations
- [ ] External API calls
- [ ] Authentication providers
- [ ] Payment processing (if applicable)

---

## Smoke Test Checklist

### Critical Path Verification
- [ ] Application loads successfully
- [ ] User can log in
- [ ] Main navigation works
- [ ] Primary user flow completes
- [ ] Data displays correctly

### Health Checks
- [ ] API health endpoints respond
- [ ] Database connectivity verified
- [ ] External service connectivity verified
- [ ] Background jobs running (if applicable)

### Post-Deployment Smoke Tests
- [ ] Production URLs accessible
- [ ] SSL/TLS certificates valid
- [ ] Error pages display correctly
- [ ] Logging working as expected

---

## Automation Coverage

### Test Suite Status

| Test Type | Total Tests | Passing | Failing | Skipped | Coverage |
|-----------|-------------|---------|---------|---------|----------|
| Unit Tests | | | | | |
| Integration Tests | | | | | |
| E2E Tests | | | | | |
| Performance Tests | | | | | |

### Automation Checklist
- [ ] All automated tests passing
- [ ] No flaky tests in critical paths
- [ ] New features covered by automated tests
- [ ] Test coverage meets minimum threshold
- [ ] Performance benchmarks within acceptable range

### Known Test Gaps
_Document any areas not covered by automation that require manual testing._

| Area | Reason | Manual Test Plan |
|------|--------|------------------|
| | | |

---

## Security Testing

### Security Checklist
- [ ] Security scan completed (SAST)
- [ ] Dependency vulnerability scan completed
- [ ] No critical/high vulnerabilities unresolved
- [ ] Authentication/authorization tested
- [ ] Input validation verified
- [ ] Sensitive data handling reviewed

---

## Performance Testing

### Performance Checklist
- [ ] Load testing completed
- [ ] Response times within SLA
- [ ] No memory leaks detected
- [ ] Database query performance verified
- [ ] API response times acceptable

### Performance Metrics

| Metric | Target | Actual | Status |
|--------|--------|--------|--------|
| Page Load Time | | | |
| API Response Time | | | |
| Concurrent Users | | | |
| Error Rate | | | |

---

## Accessibility Testing

### Accessibility Checklist
- [ ] Screen reader compatibility tested
- [ ] Keyboard navigation verified
- [ ] Color contrast requirements met
- [ ] ARIA labels present where needed
- [ ] WCAG 2.1 AA compliance verified

---

## Sign-off Procedure

### Pre-Sign-off Requirements
- [ ] All critical bugs resolved
- [ ] All high-priority bugs resolved or deferred with approval
- [ ] Test summary report completed
- [ ] Known issues documented
- [ ] Release notes reviewed for accuracy

### Sign-off Authority

| Environment | Sign-off By | Date | Signature |
|-------------|------------|------|-----------|
| Development | | | |
| Staging | | | |
| Production | | | |

### QA Lead Sign-off

I, _________________________, confirm that:

- [ ] All planned testing has been completed
- [ ] All critical and high-priority bugs have been resolved
- [ ] The release meets quality standards
- [ ] Known issues have been documented and accepted by Product Owner

**QA Lead Name**: _______________________

**Date**: _______________________

**Signature**: _______________________

---

## Test Summary Report

### Release Information
- **Release Version**: 
- **Release Date**: 
- **QA Lead**: 

### Testing Summary
- **Total Test Cases Executed**: 
- **Passed**: 
- **Failed**: 
- **Blocked**: 
- **Not Executed**: 

### Bug Summary
- **Critical**: 
- **High**: 
- **Medium**: 
- **Low**: 

### Recommendation
- [ ] Ready for release
- [ ] Ready with known issues
- [ ] Not ready for release

### Notes
_Add any additional notes or observations here._

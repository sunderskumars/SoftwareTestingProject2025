# Software Testing Project for app.vwo.com

## Table of Contents
- [Project Overview](#project-overview)
- [Test Plan](#test-plan)
- [Test Scenarios](#test-scenarios)
- [Test Execution](#test-execution)
- [Test Deliverables](#test-deliverables)
- [Tools Used](#tools-used)
- [Risk and Mitigation](#risk-and-mitigation)
- [Test Results](#test-results)
- [Conclusion](#conclusion)

## Project Overview
This repository contains the test plan, test cases, and related documentation for the software testing project of **app.vwo.com**, a platform for conducting A/B testing on websites. The goal is to ensure the system functions as expected across various scenarios, environments, and devices. Testing will focus on critical features like login, dashboard, A/B campaign creation, user experience, performance, security, and accessibility.

## Test Plan
The test plan outlines the strategy, scope, objectives, resources, and schedule for testing the app.vwo.com platform.

### Key Components:
- **Objective**: Ensure features like login, dashboard, account creation, and A/B testing campaigns work as expected.
- **Scope**: Covers functional, non-functional, UI/UX, cross-browser, and security testing.
- **Test Strategy**: Involves both manual and automated testing, with a focus on critical user journeys.
- **Test Environment**: Includes multiple OS, browsers, and device configurations.
- **Risk Mitigation**: Plans for handling environment issues, resource availability, and time constraints.

For further details, see the [Test Plan](test_plan.md).

## Test Scenarios
The test scenarios describe the specific conditions under which tests will be executed.

### Example Test Scenarios:
- **Login Page**: Test successful login, invalid login attempts, session timeout.
- **Dashboard**: Test loading of widgets, editing campaign details, user profile management.
- **Create Campaign**: Test creating and managing A/B tests, defining variants, and launching tests.

For detailed scenarios, refer to the [Test Cases](test_cases.md).

## Test Execution
Test execution involves running the defined test cases on various configurations and logging the results.

- **Manual Testing**: Execution of test cases by QA team members on different browsers and devices.
- **Automated Testing**: Execution of automated regression tests using Selenium and TestNG.
- **Performance Testing**: Load testing using JMeter to simulate 1000 concurrent users.
- **Security Testing**: OWASP Top 10 compliance checks.

## Test Deliverables
- **Test Cases**: Detailed test cases for all functional and non-functional aspects.
- **Defect Reports**: Logs of defects found, including severity and priority.
- **Test Summary Report**: Overall testing results, defect resolution status, and closure.
- **Traceability Matrix**: Mapping of requirements to test cases to ensure complete coverage.

## Tools Used
- **JIRA**: Bug tracking and task management.
- **Selenium**: UI automation.
- **TestNG**: Automation framework for test execution.
- **JMeter**: Performance testing tool for load testing.
- **Postman**: API testing.
- **BrowserStack**: Cross-browser and device testing.
- **Axe / Lighthouse**: Accessibility testing.

## Risk and Mitigation
### Potential Risks:
1. **Environment Downtime**: Delays in the availability of test environments.
   - **Mitigation**: Use backup environments or simulate test data.
2. **Shortened Testing Window**: Limited time for comprehensive testing.
   - **Mitigation**: Prioritize tests using a risk-based approach and focus on critical functionalities.
3. **Integration Issues**: Problems with third-party services affecting campaigns.
   - **Mitigation**: Mock third-party services and validate core functionality first.

## Test Results
### Summary of Test Execution:
- **Total Test Cases**: 120  
- **Passed**: 95  
- **Failed**: 15  
- **Defects Found**: 10 (6 fixed, 4 in progress)

### Key Defects:
- Login page session timeout issue.
- Dashboard widget layout breaking on mobile devices.
- A/B test creation UI bug on Safari.

## Conclusion
The testing project has successfully verified the core functionality of **app.vwo.com**. While there are some issues in specific areas (mainly UI and performance), these have been logged and are being prioritized for resolution. Automation has significantly reduced regression testing time, and performance testing confirms the system's readiness for up to 1000 concurrent users.

The application is mostly stable for production, and we recommend a final round of UAT (User Acceptance Testing) before the next release.

---

### References
- [Test Plan](test_plan.md)
- [Test Cases](test_cases.md)
- [JIRA](https://jira.example.com) (Bug Tracking System)

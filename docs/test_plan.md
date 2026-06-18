# Test Plan: Automation Testing for Automation Exercise Web Application

## 1. Introduction & Project Goal
The goal of this project is to develop a comprehensive test automation system (UI and API) for the educational e-commerce platform `automationexercise.com`. 
This project demonstrates the application of modern QA practices, design patterns, and test integration into a CI/CD pipeline.

## 2. Scope of Testing
The target of testing is the web application and its public API.

### In Scope:
- **Documentation:** Creation of checklists and test cases for critical functionality.
- **API Testing:** Coverage of endpoints.
- **UI Testing:** Automation of key user scenarios.
- **Functional Modules:**
  - User registration and authentication.
  - Product search, filtering, and browsing.
  - Cart management.
  - Checkout process and payment.
- **Performance Testing:** Demonstration of API performance and load testing using Locust
- **Security Testing:** Basic security audit of API and HTTP response headers using custom Python scripts.
- **Cross-Browser Testing:** Execution of UI tests across multiple browser engines (Chromium and Firefox).
- **Infrastructure:** CI/CD pipeline setup for automated test execution and Allure report generation.

### Out of Scope:
- High-load stress and spike testing that could potentially cause a DDoS condition on the third-party resource.
- Deep manual penetration testing and advanced vulnerability assessment.

## 3. Strategy & Technology Stack
Testing is split into multiple levels to ensure high execution speed, stability, and broad coverage:
1. **API Level:** Fast verification of business logic, status codes, and response structures.
2. **UI Level:** Emulation of real user behavior in different browser environments.
3. **Performance Level:** Assessing endpoint behavior under simulated multi-user traffic.
4. **Security Level:** Automated checks for missing security headers.

### Technology Stack:
- **Language:** Python 3.11+
- **Framework:** Pytest 
- **UI Driver:** Playwright 
- **API Client:** Requests
- **Performance Tool:** Locust
- **Design Patterns:** Page Object Model (POM) for UI tests
- **Data Generation:** Faker library
- **Reporting:** Allure Framework
- **CI/CD:** GitHub Actions

## 4. Acceptance Criteria

### Suspension Criteria:
- Availability and stability of the `automationexercise.com` website and its API.
- Fully configured and structured local repository.

### Exit Criteria:
- Basic checklists and critical test cases are documented.
- At least 80% of planned critical E2E and API scenarios are automated.
- UI tests pass successfully in both Chromium and Firefox environments.
- Performance scripts execute without HTTP failure rates exceeding 1%.
- Automated GitHub Actions pipeline triggers on every push to the `main` branch.
- Allure reports generate successfully with zero "Broken" statuses caused by automation framework issues.

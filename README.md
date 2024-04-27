# Qubika Sports Club Management System E2E Tests

## Description
This project contains end-to-end automated tests for the Qubika Sports Club Management System using Playwright. It is designed to ensure the application performs as expected from a user's perspective through automated user interaction tests across multiple pages.

### Key Features Tested
- **User Authentication**: Ensures that the user login mechanism is secure and reliable.
- **Category Management**: Tests the ability to add, modify, and delete category data accurately.
- **Integration Points**: Verifies that all external system integrations perform as expected under various scenarios.

## Enhancements and Updates

### Recent Enhancements
- **Improved Test Coverage**: Expanded tests to cover new features like online bookings and event notifications.
- **Performance Optimization**: Reduced test execution time by optimizing test flows and leveraging parallel test executions.
- **Enhanced Debugging Capabilities**: Integrated Playwright’s trace viewer for better debugging of test cases.

### Planned Enhancements
- **Continuous Integration**: Setup a CI/CD pipeline to automatically run tests on every commit, ensuring immediate feedback on the impact of changes.
- **Cross-Browser Testing**: Extend testing to cover all major browsers to ensure consistency across user platforms.
- **Accessibility Tests**: Introduce accessibility checks to ensure the application is usable by people with disabilities.

## Prerequisites
To run these tests, you must have the following installed:
- Node.js (LTS version recommended)
- npm (Node Package Manager)

## Installation

Follow these steps to set up the Playwright test environment on your local machine:

1. **Clone the Repository**
   ```bash
   git clone https://your-repository-url.git
   cd your-repository-directory
Install Dependencies
bash
Copy code
npm install
Install Playwright
This will install Playwright and browser binaries for Chromium, Firefox, and WebKit.
bash
Copy code
npx playwright install
Configuration

.env File: Ensure that all necessary environment variables are set up in a .env file or directly in your environment, which might include API endpoints, user credentials, etc.
Running Tests

To run all tests:
bash

npx playwright test
To run a specific test file:
bash

npx playwright test path/to/test/file.spec.ts
To run tests with a visual browser (headed mode):
bash

npx playwright test --headed
Debugging Tests

To debug tests using Playwright's trace viewer:
bash

npx playwright show-report
To run tests in debug mode:
bash

npx playwright test --debug
Test Structure

Test files: Tests are located in the tests folder.
Helper functions: Utility functions like generateRandomEmail and generateRandomString are defined in the test files or a separate utilities module.
Continuous Integration

If applicable, provide instructions on how to integrate and run these tests in a CI/CD pipeline.
Contributing

Example File Structure
lua
project-root/
│
├── tests/
│   ├── authentication.spec.ts
│   └── category-management.spec.ts
│
├── playwright.config.ts
├── package.json
├── .env
└── README.md

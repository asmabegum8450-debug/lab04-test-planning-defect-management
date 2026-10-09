# Test Plan: Counter Application

## 1. Test Objectives

1. Verify that the Counter application displays the correct initial count.
2. Verify that Increment, Decrement, and Reset update the count correctly.

## 2. Scope

### In Scope
- Initial count of zero.
- Increment button behavior.
- Decrement button behavior.
- Reset button behavior.
- Sequences of multiple button clicks.

### Out of Scope
- User authentication.
- Database integration and persistence.
- Network and API testing.
- Performance and security testing.

## 3. Testing Approach

Manual functional testing will be performed by interacting with the application in a browser. The source code will also be reviewed to identify incorrect button behavior. Test results will be recorded for each test case.

## 4. Test Environment and Tools

- Operating system: macOS
- Application: React and TypeScript Counter application
- Development server: Vite
- Browser: Chrome
- Tools: Terminal, text editor, Git, and GitHub

## 5. Product Risks

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Decrement increases the count instead of decreasing it | High | Medium | Test decrement from zero and from a positive value |
| Reset does not return the count to zero | Low | Medium | Test reset after multiple changes |
| Repeated clicks produce an incorrect count | Medium | Medium | Test sequences of increment and decrement actions |

## 6. Entry Criteria

1. Application dependencies are installed successfully.
2. The Counter application starts in the test environment.
3. The test cases have been documented.
4. The application can be opened in a browser.

## 7. Exit Criteria

1. All five documented test cases have been executed.
2. Every failed test has a documented result.
3. All identified defects have a report with severity and priority.
4. Test results and the final defect report are committed to GitHub.

## 8. Test Deliverables

- Test plan
- Test case and execution report
- Defect report
- GitHub repository containing the project and documentation


# SauceDemo Manual Test Plan

## Objective
Assess the main shopping journey and document any issues found
through manual testing.

## Application
https://www.saucedemo.com/

## Scope
- Login with valid, invalid and empty credentials
- Product listing and sorting
- Product details
- Adding and removing basket items
- Checkout field validation
- Order totals and order completion
- Logout

## Out of Scope
- Real payments and deliveries
- Load and performance testing
- Security penetration testing
- Automated testing in this phase

## Approach
- Prioritise the complete login-to-checkout journey.
- Include positive and negative test cases.
- Use equivalence partitioning for valid, invalid and empty inputs.
- Explore unexpected actions and navigation.
- Retest reported defects and check related features.

## Test Environment
Record the following before each test run:
- Date
- Operating system
- Browser and version
- Test account
- Relevant setup or starting state

Use demo accounts provided by the application.
Start independent tests with a clean basket.

## Deliverables
- Test cases with steps and expected results
- Execution results with actual outcomes
- Bug reports with reproduction steps and evidence
- Test summary with findings and limitations

## Entry Criteria
- The application is accessible.
- Demo accounts are available.
- Test cases and expected outcomes are documented.

## Completion Criteria
- All planned high-priority tests have been attempted.
- Each attempted test has a recorded result.
- Defects include reproduction steps and evidence.
- Blocked and untested areas are listed in the summary.

## Risks and Limitations
- The demo application may change or become unavailable.
- Some demo accounts may intentionally exhibit faulty behaviour.
  Record the account used and identify these as demo findings.
- Expected behaviour is based on the visible shopping flow;
  assumptions must be documented where requirements are unavailable.

## Status
Draft plan. Execution results will be added after testing.

# Test Plan: SauceDemo Manual Testing

## Objective

Verify that a customer can authenticate, browse products, manage a cart, complete checkout, and end a session without critical defects.

## Scope

### In Scope

- Login and error handling
- Product catalogue and sorting
- Product details
- Cart operations
- Checkout validation and successful order placement
- Logout

### Out of Scope

- Payment gateway integration
- Performance and load testing
- Accessibility testing
- Cross-browser coverage beyond Google Chrome
- Security penetration testing

## Test Approach

- Execute smoke testing after a new build or deployment.
- Execute regression testing before a release.
- Use equivalence partitioning for required checkout fields.
- Record confirmed defects with evidence in the `bug-reports/` directory.

## Test Environment

| Parameter | Value |
| --- | --- |
| Application | SauceDemo |
| URL | https://www.saucedemo.com/ |
| Browser | Google Chrome, latest stable version |
| Operating system | Windows 11 |
| Test account | `standard_user` / `secret_sauce` |

## Entry Criteria

- The application is available over HTTPS.
- Test accounts are available.
- The build is deployed to the test environment.

## Exit Criteria

- All critical and high-priority test cases are executed.
- No unresolved critical defects remain.
- Test results and confirmed defects are documented.

## Risks

| Risk | Impact | Mitigation |
| --- | --- | --- |
| Shared public test environment changes unexpectedly | Medium | Record execution date, time, and exact observed behaviour. |
| Public test accounts are unavailable | High | Verify credentials before execution and record blocked cases. |
| Browser update changes rendering or behaviour | Low | Record browser version in the test summary. |


<div align="center">

# SauceDemo Manual Testing Portfolio

Manual QA documentation for the [SauceDemo](https://www.saucedemo.com/) demo e-commerce application

</div>

## Project Contents

| Directory or file | Description |
| --- | --- |
| `test-cases/` | Detailed functional test cases in Markdown. |
| `checklists/` | Smoke and regression checklists. |
| `bug-reports/` | Bug-report template and screenshot storage rules. |
| `test-plan.md` | Scope, approach, environment, risks, and entry and exit criteria. |
| `test-summary.md` | Execution report template with transparent result tracking. |

## System Under Test

- Application: SauceDemo
- URL: https://www.saucedemo.com/
- Domain: e-commerce
- Main flows: authentication, product catalogue, cart, checkout, and logout

## Test Design Coverage

- Positive and negative authentication
- Product sorting
- Cart management
- Checkout validation
- Successful order placement
- Session termination

## How to Use This Repository

1. Select the relevant checklist for the required test level.
2. Execute the test cases against the stated environment.
3. Record the actual result and status in `test-summary.md`.
4. Create one Markdown file per confirmed defect from `bug-reports/bug-report-template.md`.
5. Store evidence in `bug-reports/screenshots/` and link it from the bug report.

## Notes

The test summary contains only observed results from the recorded manual execution. No defects are added unless they are reproduced and documented with evidence.

# Test Summary

## Execution Status

Full manual test run completed successfully on 2026-10-27.

## Environment

| Parameter | Value |
| --- | --- |
| Application | SauceDemo |
| URL | https://www.saucedemo.com/ |
| Browser | Codex In-app Browser, Chromium engine |
| Operating system | Windows 11 |
| Execution date | 2026-10-27 |

## Results

| Metric | Value |
| --- | --- |
| Planned test cases | 15 |
| Executed | 15 |
| Passed | 15 |
| Failed | 0 |
| Blocked | 0 |
| Not run | 0 |

## Executed Test Cases

| ID | Result | Evidence |
| --- | --- | --- |
| TC-LOGIN-001 | Passed | Products page opened after valid login. |
| TC-LOGIN-002 | Passed | Incorrect-password error message was displayed. |
| TC-LOGIN-003 | Passed | Locked-out-user error message was displayed. |
| TC-CATALOG-001 | Passed | Prices were ordered as $7.99, $9.99, $15.99, $15.99, $29.99, and $49.99. |
| TC-CATALOG-002 | Passed | Product details showed the correct name, description, price, image, and add-to-cart button. |
| TC-CART-001 | Passed | Sauce Labs Backpack appeared in the cart with quantity 1 and price $29.99. |
| TC-CART-002 | Passed | Product was removed and the cart became empty. |
| TC-CART-003 | Passed | Continue Shopping returned to the catalogue and preserved the cart item. |
| TC-CHECKOUT-001 | Passed | Checkout opened the Checkout: Your Information page. |
| TC-CHECKOUT-002 | Passed | `First Name is required` validation message was displayed. |
| TC-CHECKOUT-003 | Passed | `Last Name is required` validation message was displayed. |
| TC-CHECKOUT-004 | Passed | `Postal Code is required` validation message was displayed. |
| TC-CHECKOUT-005 | Passed | Confirmation page displayed `Thank you for your order!`. |
| TC-CHECKOUT-006 | Passed | Cancel returned the user to the cart with Sauce Labs Backpack retained. |
| TC-SESSION-001 | Passed | Logout returned the user to the login page. |

## Confirmed Defects

No confirmed defects were found during the executed scenarios. Add a separate Markdown file to `bug-reports/` after reproducing and documenting an issue.

## Extended Regression Checks

| Check | Result | Evidence |
| --- | --- | --- |
| Name A-Z sorting | Passed | Products were displayed as Sauce Labs Backpack, Sauce Labs Bike Light, Sauce Labs Bolt T-Shirt, Sauce Labs Fleece Jacket, Sauce Labs Onesie, and Test.allTheThings() T-Shirt (Red). |
| Multiple-product cart | Passed | Cart badge showed 2 and contained Sauce Labs Backpack and Sauce Labs Bike Light. |

## Completion Status

All 15 test cases, all smoke checks, and all regression checks in this repository have been executed. Repeat the suite after future application changes and create bug reports with screenshots for every confirmed defect.

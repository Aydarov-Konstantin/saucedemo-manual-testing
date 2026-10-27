# Regression Testing Checklist

| Area | Check | Status | Notes |
| --- | --- | --- | --- |
| Authentication | Valid login | Passed | 2026-10-27 |
| Authentication | Invalid password error | Passed | 2026-10-27 |
| Authentication | Locked-out user error | Passed | 2026-10-27 |
| Catalogue | Product names, prices, and images are visible | Passed | 2026-10-27 |
| Catalogue | Sort by name and price | Passed | Name A-Z and price low-to-high sorting were verified. |
| Product details | Details match the selected product | Passed | Sauce Labs Backpack details were verified. |
| Cart | Add one and multiple products | Passed | One-product and two-product cart flows were verified. |
| Cart | Remove a product | Passed | 2026-10-27 |
| Cart | Cart badge count is correct | Passed | Badge changed from 1 to empty after removal. |
| Checkout | Required-field validation | Passed | First name, last name, and postal code validation were verified. |
| Checkout | Item list and totals are correct | Passed | Backpack price $29.99, tax $2.40, total $32.39. |
| Checkout | Successful order completion | Passed | 2026-10-27 |
| Checkout | Cancel returns user to the cart | Passed | Cart content was retained after cancellation. |
| Session | Logout returns user to the login page | Passed | 2026-10-27 |

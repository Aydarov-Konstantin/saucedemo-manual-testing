# SauceDemo Test Cases

## Test Environment

- Application URL: https://www.saucedemo.com/
- Test account: `standard_user` / `secret_sauce`
- Browser: Google Chrome, latest stable version

| ID | Title | Preconditions | Steps | Expected Result | Priority |
| --- | --- | --- | --- | --- | --- |
| TC-LOGIN-001 | Sign in with valid credentials | Login page is open | 1. Enter `standard_user`.<br>2. Enter `secret_sauce`.<br>3. Click **Login**. | The Products page opens and the product catalogue is visible. | High |
| TC-LOGIN-002 | Sign in with an invalid password | Login page is open | 1. Enter `standard_user`.<br>2. Enter an invalid password.<br>3. Click **Login**. | An error message states that the username and password do not match. | High |
| TC-LOGIN-003 | Sign in as a locked-out user | Login page is open | 1. Enter `locked_out_user`.<br>2. Enter `secret_sauce`.<br>3. Click **Login**. | An error message states that the user has been locked out. | High |
| TC-CATALOG-001 | Sort products by price from low to high | User is signed in | 1. Open the sorting control.<br>2. Select **Price (low to high)**. | Products are displayed in ascending price order. | Medium |
| TC-CATALOG-002 | Open product details | User is signed in | 1. Click a product name or image. | Product details page shows the correct name, description, price, image, and add-to-cart button. | Medium |
| TC-CART-001 | Add one product to the cart | User is signed in | 1. Click **Add to cart** for Sauce Labs Backpack.<br>2. Open the cart. | The cart contains Sauce Labs Backpack with its correct price and quantity. | High |
| TC-CART-002 | Remove a product from the cart | Cart contains Sauce Labs Backpack | 1. Click **Remove** for Sauce Labs Backpack. | The product is removed and the cart becomes empty. | High |
| TC-CART-003 | Continue shopping from the cart | Cart contains at least one product | 1. Click **Continue Shopping**. | User returns to the Products page and the cart contents are retained. | Medium |
| TC-CHECKOUT-001 | Start checkout from the cart | Cart contains at least one product | 1. Open the cart.<br>2. Click **Checkout**. | The Checkout: Your Information page opens. | High |
| TC-CHECKOUT-002 | Validate required first name | Checkout information page is open | 1. Leave all fields empty.<br>2. Click **Continue**. | An error message states that first name is required. | High |
| TC-CHECKOUT-003 | Validate required last name | Checkout information page is open | 1. Enter a first name.<br>2. Leave last name and postal code empty.<br>3. Click **Continue**. | An error message states that last name is required. | High |
| TC-CHECKOUT-004 | Validate required postal code | Checkout information page is open | 1. Enter first and last names.<br>2. Leave postal code empty.<br>3. Click **Continue**. | An error message states that postal code is required. | High |
| TC-CHECKOUT-005 | Complete an order | Cart contains Sauce Labs Backpack | 1. Start checkout.<br>2. Enter valid first name, last name, and postal code.<br>3. Click **Continue**.<br>4. Verify item and totals.<br>5. Click **Finish**. | The order confirmation page shows `Thank you for your order!`. | Critical |
| TC-CHECKOUT-006 | Cancel checkout | Checkout information page is open | 1. Click **Cancel**. | User returns to the cart and cart contents are retained. | Medium |
| TC-SESSION-001 | Log out from the application | User is signed in | 1. Open the menu.<br>2. Click **Logout**. | User returns to the login page. | Medium |


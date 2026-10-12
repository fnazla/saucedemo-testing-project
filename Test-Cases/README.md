
## Saucedemo manual test cases
## Execution note
- Application: https://www.saucedemo.com/
- Start each test logged out and on the login page.
- Use the current demo credentials displayed on the application.
- These cases are not yet executed.
- Record actual results separately after running each test.

## TC-001: Login with valid credentials
**Priority:** High  
**Type:** Positive  
**Precondition:** Login page is open.

**Test Data**
- Username: standard_user
- Password: secret_sauce

**Steps**
1. Enter the username.
2. Enter the correct demo password.
3. Click Login.

**Expected Result**
The product inventory page opens and the product list is displayed.

## TC-002: Login with an incorrect password
**Priority:** High  
**Type:** Negative  
**Precondition:** Login page is open.

**Test Data**
- Username: standard_user
- Password: incorrect_password_123

**Steps**
1. Enter the username.
2. Enter the incorrect password.
3. Click Login.

**Expected Result**
Login is refused, an error message is displayed, and the user
remains on the login page.

## TC-003: Login with an empty username
**Priority:** Medium  
**Type:** Negative  
**Precondition:** Login page is open.

**Steps**
1. Leave the username field empty.
2. Enter the correct demo password (secret_sauce).
3. Click Login.

**Expected Result**
Login is refused and a validation message indicates that
a username is required.

## TC-004: Login with an empty password
**Priority:** Medium  
**Type:** Negative  
**Precondition:** Login page is open.

**Steps**
1. Enter standard_user as the username.
2. Leave the password field empty.
3. Click Login.

**Expected Result**
Login is refused and a validation message indicates that
a password is required.

## TC-005: Login with both fields empty
**Priority:** Medium  
**Type:** Negative  
**Precondition:** Login page is open.

**Steps**
1. Leave both username and password fields empty.
2. Click Login.

**Expected Result**
Login is refused and a required-field validation message
is displayed. The user remains on the login page.

## TC-006: Add a product to the basket
**Priority:** High
**Type:** Positive
**Precondition:** Logged in as standard_user with an empty basket.

**Steps**
1. Note the name and price of a product.
2. Click its Add to cart button.
3. Check the basket badge.
4. Open the basket.

**Expected Result**
- The basket badge shows 1.
- The selected product appears in the basket.
- Its name and price match the product listing.
- Its quantity is 1.

## TC-007: Remove a product from the basket
**Priority:** High
**Type:** Positive
**Precondition:** Logged in as standard_user with exactly one
product in the basket.

**Steps**
1. Open the basket.
2. Click Remove beside the product.
3. Check the basket contents and badge.

**Expected Result**
- The product is removed.
- The basket is empty.
- The basket badge no longer displays an item count.

## TC-008: Checkout with an empty first name
**Priority:** High
**Type:** Negative
**Precondition:** Logged in as standard_user with one product
in the basket, on the checkout information page.

**Steps**
1. Leave First Name empty.
2. Enter Tester in Last Name.
3. Enter SG5 1AA in Postal Code.
4. Click Continue.

**Expected Result**
A message indicates that First Name is required.
The user remains on the checkout information page.

## TC-009: Checkout with an empty last name
**Priority:** High
**Type:** Negative
**Precondition:** Logged in as standard_user with one product
in the basket, on the checkout information page.

**Steps**
1. Enter Test in First Name.
2. Leave Last Name empty.
3. Enter SG5 1AA in Postal Code.
4. Click Continue.

**Expected Result**
A message indicates that Last Name is required.
The user remains on the checkout information page.

## TC-010: Checkout with an empty postal code
**Priority:** High
**Type:** Negative
**Precondition:** Logged in as standard_user with one product
in the basket, on the checkout information page.

**Steps**
1. Enter Test in First Name.
2. Enter Tester in Last Name.
3. Leave Postal Code empty.
4. Click Continue.

**Expected Result**
A message indicates that Postal Code is required.
The user remains on the checkout information page.

## TC-011: Complete an order
**Priority:** High
**Type:** Positive
**Precondition:** Logged in as standard_user with exactly one
product in the basket. Record its name and price.

**Steps**
1. Open the basket and click Checkout.
2. Enter Test, Tester and SG5 1AA in the required fields.
3. Click Continue.
4. Check the product name, price and quantity.
5. Check that Item total matches the product price.
6. Check that Total equals Item total plus the displayed Tax.
7. Click Finish.

**Expected Result**
- The overview shows the correct product and quantity 1.
- The item total and final total are calculated correctly.
- An order confirmation is displayed after clicking Finish.

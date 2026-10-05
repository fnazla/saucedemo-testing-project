
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
- Password: Use the demo password displayed on the login page.

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
2. Enter the correct demo password.
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

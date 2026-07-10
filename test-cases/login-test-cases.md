# Test Cases — Login Feature

**Application:** SauceDemo — https://www.saucedemo.com  
**Prepared by:** Alison Kate  
**Date:** July 2026  
**Feature:** User Login  

---

## Summary

| Total Test Cases | Passed | Failed | Blocked |
|-----------------|--------|--------|---------|
| 8 | - | - | - |

---

## Test Cases

### TC-001 — Login with valid credentials

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-001 |
| **Feature** | Login |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Enter username: `standard_user`
3. Enter password: `secret_sauce`
4. Click the Login button

**Expected Result:** User is redirected to the product listing page

---

### TC-002 — Login with invalid password

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-002 |
| **Feature** | Login |
| **Test Type** | Negative |
| **Priority** | High |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Enter username: `standard_user`
3. Enter password: `wrongpassword`
4. Click the Login button

**Expected Result:** Error message displayed — "Username and password do not match"

---

### TC-003 — Login with empty username

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-003 |
| **Feature** | Login |
| **Test Type** | Negative |
| **Priority** | High |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Leave username blank
3. Enter password: `secret_sauce`
4. Click the Login button

**Expected Result:** Error message displayed — "Username is required"

---

### TC-004 — Login with empty password

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-004 |
| **Feature** | Login |
| **Test Type** | Negative |
| **Priority** | High |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Enter username: `standard_user`
3. Leave password blank
4. Click the Login button

**Expected Result:** Error message displayed — "Password is required"

---

### TC-005 — Login with both fields empty

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-005 |
| **Feature** | Login |
| **Test Type** | Negative |
| **Priority** | Medium |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Leave both fields blank
3. Click the Login button

**Expected Result:** Error message displayed — "Username is required"

---

### TC-006 — Login with locked out user

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-006 |
| **Feature** | Login |
| **Test Type** | Negative |
| **Priority** | High |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Enter username: `locked_out_user`
3. Enter password: `secret_sauce`
4. Click the Login button

**Expected Result:** Error message displayed — "Sorry, this user has been locked out"

---

### TC-007 — Login with invalid username

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-007 |
| **Feature** | Login |
| **Test Type** | Negative |
| **Priority** | Medium |
| **Precondition** | User is on the login page |

**Steps:**
1. Open https://www.saucedemo.com
2. Enter username: `unknown_user`
3. Enter password: `secret_sauce`
4. Click the Login button

**Expected Result:** Error message displayed — "Username and password do not match"

---

### TC-008 — Logout from the application

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-008 |
| **Feature** | Login |
| **Test Type** | Positive |
| **Priority** | Low |
| **Precondition** | User is logged in as standard_user |

**Steps:**
1. Click the hamburger menu (top left)
2. Click Logout

**Expected Result:** User is redirected back to the login page
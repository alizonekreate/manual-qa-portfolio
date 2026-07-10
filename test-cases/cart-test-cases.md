# Test Cases — Shopping Cart Feature

**Application:** SauceDemo — https://www.saucedemo.com  
**Prepared by:** Alison Kate Lachica 
**Date:** July 2026  
**Feature:** Shopping Cart  

---

## Summary

| Total Test Cases | Passed | Failed | Blocked |
|-----------------|--------|--------|---------|
| 10 | - | - | - |

---

## Test Cases

### TC-009 — Add a single item to the cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-009 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User is logged in as standard_user |

**Steps:**
1. On the product listing page, click "Add to cart" on any product
2. Check the cart icon on the top right

**Expected Result:** Cart icon shows badge with number 1

---

### TC-010 — Add multiple items to the cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-010 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User is logged in as standard_user |

**Steps:**
1. Click "Add to cart" on three different products
2. Check the cart icon on the top right

**Expected Result:** Cart icon shows badge with number 3

---

### TC-011 — Remove an item from the product listing page

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-011 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User has at least one item in the cart |

**Steps:**
1. On the product listing page, click "Remove" on an item already in the cart
2. Check the cart icon on the top right

**Expected Result:** Cart badge count decreases by 1

---

### TC-012 — View cart contents

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-012 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User has at least one item in the cart |

**Steps:**
1. Click the cart icon on the top right

**Expected Result:** Cart page opens and shows all added items with correct names and prices

---

### TC-013 — Remove an item from the cart page

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-013 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User is on the cart page with at least one item |

**Steps:**
1. Click "Remove" next to any item on the cart page
2. Check the remaining items in the cart

**Expected Result:** Item is removed and no longer displayed in the cart

---

### TC-014 — Remove all items from the cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-014 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | Medium |
| **Precondition** | User has multiple items in the cart |

**Steps:**
1. On the cart page, click "Remove" on every item one by one
2. Check the cart icon after all items are removed

**Expected Result:** Cart is empty and badge disappears from the cart icon

---

### TC-015 — Continue shopping from cart page

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-015 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | Medium |
| **Precondition** | User is on the cart page |

**Steps:**
1. Click the "Continue Shopping" button

**Expected Result:** User is returned to the product listing page and cart contents are preserved

---

### TC-016 — Proceed to checkout from cart page

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-016 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | High |
| **Precondition** | User has at least one item in the cart |

**Steps:**
1. On the cart page, click the "Checkout" button

**Expected Result:** User is taken to the checkout information form

---

### TC-017 — Cart is empty on first login

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-017 |
| **Feature** | Shopping Cart |
| **Test Type** | Positive |
| **Priority** | Medium |
| **Precondition** | User has just logged in for the first time in the session |

**Steps:**
1. Log in as standard_user
2. Click the cart icon

**Expected Result:** Cart page shows no items and displays "Your cart is empty" or similar message

---

### TC-018 — Cart does not persist after logout and login

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-018 |
| **Feature** | Shopping Cart |
| **Test Type** | Negative |
| **Priority** | Medium |
| **Precondition** | User has items in the cart |

**Steps:**
1. Add at least one item to the cart
2. Logout from the application
3. Log back in as standard_user
4. Click the cart icon

**Expected Result:** Cart is empty — items do not persist between sessions
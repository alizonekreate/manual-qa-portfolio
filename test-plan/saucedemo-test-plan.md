# Test Plan — SauceDemo

**Version:** 1.0  
**Prepared by:** Alison Kate  
**Date:** July 2026  
**Application:** SauceDemo — https://www.saucedemo.com  

---

## 1. Objective

The goal of this test plan is to verify that the core features of 
SauceDemo work correctly from a user's perspective. This includes 
login, product browsing, cart management, and the checkout process.

---

## 2. Scope

### In Scope
- Login and logout functionality
- Product listing page — display, sorting, and navigation
- Shopping cart — adding and removing items
- Checkout flow — form validation and order completion

### Out of Scope
- Performance testing
- Security testing
- Mobile responsiveness
- Payment gateway (SauceDemo does not have a real payment system)

---

## 3. Test Approach

Testing will be done manually by navigating the application as an 
end user. Both positive and negative test cases will be written and 
executed. Bugs found will be logged in the bug-reports folder.

---

## 4. Features to Test

| Feature | Priority |
|---------|----------|
| Login with valid credentials | High |
| Login with invalid credentials | High |
| Product listing and sort order | Medium |
| Add item to cart | High |
| Remove item from cart | High |
| Checkout with valid details | High |
| Checkout with missing fields | Medium |
| Logout | Low |

---

## 5. Test Environment

| Item | Details |
|------|---------|
| Application URL | https://www.saucedemo.com |
| Browser | Google Chrome (latest) |
| Test Account | standard_user / secret_sauce |
| Operating System | Windows |
| Testing Type | Manual — Functional |

---

## 6. Test Data

| Username | Password | Expected Result |
|----------|----------|-----------------|
| standard_user | secret_sauce | Login successful |
| locked_out_user | secret_sauce | Login blocked with error |
| invalid_user | invalid_pass | Login fails with error |

---

## 7. Entry and Exit Criteria

### Entry Criteria
- Application is accessible and loading correctly
- Test account credentials are working
- Test cases have been written and reviewed

### Exit Criteria
- All high priority test cases have been executed
- All critical bugs have been logged
- Test summary report has been completed

---

## 8. Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| App is down or unavailable | Testing blocked | Reschedule and retry |
| Test account stops working | Cannot log in | Use alternative SauceDemo accounts |

---

## 9. Deliverables

- Test cases — located in `test-cases/`
- Bug reports — located in `bug-reports/`
- Test summary — located in `test-summary/`
# Test Summary Report — Sprint 1

**Application:** SauceDemo — https://www.saucedemo.com  
**Prepared by:** Alison Kate Lachica
**Date:** July 2026  
**Features Tested:** Login, Shopping Cart  

---

## Overview

This report summarizes the results of manual testing performed on 
the Login and Shopping Cart features of SauceDemo. Testing was 
conducted manually using Chrome on Windows.

---

## Test Execution Summary

| Feature | Total TCs | Passed | Failed | Blocked |
|---------|-----------|--------|--------|---------|
| Login | 8 | 8 | 0 | 0 |
| Shopping Cart | 10 | 9 | 1 | 0 |
| **Total** | **18** | **17** | **1** | **0** |

---

## Test Coverage

| Area | Status |
|------|--------|
| Valid login | Covered |
| Invalid login scenarios | Covered |
| Locked out user | Covered |
| Add items to cart | Covered |
| Remove items from cart | Covered |
| Cart persistence after logout | Covered |
| Checkout navigation | Covered |

---

## Bugs Found

| Bug ID | Feature | Summary | Severity | Status |
|--------|---------|---------|----------|--------|
| BUG-001 | Login | Locked out error message is unprofessional | Minor | Open |
| BUG-002 | Cart | Cart items persist after logout | Major | Open |

---

## Summary

Overall the application is stable and core features work as expected. 
Two bugs were identified — one minor and one major. The major bug 
(BUG-002) involves cart data persisting after logout which could be 
a data privacy concern in a real application and should be prioritized 
for fixing.

---

## Recommendations

- BUG-002 should be fixed before production release
- Error messages on the login page should be reviewed for clarity
- Additional testing on the checkout flow is recommended in the next sprint
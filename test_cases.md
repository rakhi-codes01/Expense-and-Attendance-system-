# Test Cases

**Project:** Expense, Attendance, Grading & Billing Management System

## 12.1 Normal Test Cases

| TC | Module | Input | Expected Result | Type |
|---|---|---|---|---|
| TC-01 | Menu | Choice: 1 | Expense module opens successfully | Normal |
| TC-02 | Expense | Item: Books, Category: Stationery, Amount: 250.50 | Expense added successfully | Normal |
| TC-03 | Expense | Item: Food, Category: Personal, Amount: 500 | Expense added successfully (Personal is accepted as a valid category) | Normal |
| TC-04 | Attendance | Total days: 40, Present: 32 | 80%, Eligible | Normal |
| TC-05 | Attendance | Total days: 40, Present: 30 | 75%, Eligible | Normal |
| TC-06 | Attendance | Total days: 40, Present: 29 | 72.50%, Warning | Normal |
| TC-07 | Grading | Marks: 90, 90, 90, 90, 90 | 90%, A+, PASS | Normal |
| TC-08 | Grading | Marks: 80, 80, 80, 80, 80 | 80%, A, PASS | Normal |
| TC-09 | Billing | 1 item, 500 × 1 | No discount, tax 90, total 590 | Normal |
| TC-10 | Billing | Subtotal: 1000 | 5% discount applied | Normal |
| TC-11 | Reports | Existing expense, attendance, grading and billing records | All reports displayed correctly | Normal |
| TC-12 | Main Menu | Run main.py | Main menu and project modules work successfully | Normal |

## 12.2 Edge Test Cases

| TC | Module | Input | Expected Result | Type |
|---|---|---|---|---|
| TC-13 | Menu | Invalid choice: abc | Error message and menu is displayed again | Edge Case |
| TC-14 | Expense | Amount: -50 | Rejected and re-prompted | Edge Case |
| TC-15 | Expense | Amount: 0 | Rejected and re-prompted | Edge Case |
| TC-16 | Attendance | Total days: 40, Present: 41 | Rejected and re-prompted | Edge Case |
| TC-17 | Attendance | Total days: 0 | Rejected; division by zero is prevented | Edge Case |
| TC-18 | Grading | Marks: 105 or non-numeric input | Rejected and re-prompted | Edge Case |
| TC-19 | Billing | Quantity: 0 | Rejected and re-prompted | Edge Case |
| TC-20 | Reports | Run report with no records | No records available message displayed | Edge Case |

## 12.3 Test Summary

| Test Category | Number of Cases |
|---|---:|
| Normal Test Cases | 12 |
| Edge Test Cases | 8 |
| **Total Test Cases** | **20** |

## 12.4 Testing Conclusion

The Expense, Attendance, Grading and Billing Management System is designed to be checked using 20 test cases, including 12 normal cases and 8 edge cases.

The test cases cover input validation, expense management, attendance percentage calculation, grade allocation, billing calculations and report generation. They provide a checklist for verifying the correctness and expected behavior of the major project modules.

**Note:** This document is a test-case specification. A test case should be marked *Passed* only after it has been run against the current project and the actual output has been checked against its expected result.

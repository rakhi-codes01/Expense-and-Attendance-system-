Expense, Attendance, Grading & Billing Management System

1. Project Overview

The Expense, Attendance, Grading & Billing Management System is a menu-driven Python application designed to manage four different activities in one system.

The project consists of four main modules:

1. Expense Management
2. Attendance Management
3. Student Grading System
4. Billing System

It also provides a combined Reports module to display summaries and records of all four modules.

The application uses Python functions, lists, dictionaries, loops, conditional statements and input validation to manage and process information.

2. Objectives

- To develop a menu-driven management system using Python.
- To manage and maintain expense records.
- To calculate attendance percentages and attendance status.
- To calculate student marks, grades and results.
- To generate customer invoices with discounts and taxes.
- To generate combined reports.
- To practise modular programming and input validation.

3. Technologies Used

- Programming Language: Python
- IDE: PyCharm
- Data Structures: Lists, Dictionaries and Tuples
- Concepts: Functions, Loops, Conditional Statements, Modules and Input Validation
- External Libraries: No external libraries required.

4. Project File Structure

expense_attendance_grading_billing/
│
├── main.py
├── expenses.py
├── attendance.py
├── grading.py
├── billing.py
├── reports.py
├── validators.py
├── test_project_20_cases.py
└── README.md

5. Description of Files

File Name| Description
main.py| Controls the main menu and connects all modules.
expenses.py| Adds, displays and calculates expense summaries.
attendance.py| Records attendance and calculates attendance percentages.
grading.py| Calculates student marks, percentages, grades and results.
billing.py| Generates invoices and calculates discounts and taxes.
reports.py| Generates combined reports for all modules.
validators.py| Validates integer, decimal, name and yes/no inputs.
test_project_20_cases.py| Contains 20 test cases for checking the application.

6. Main Menu

The main menu provides the following options:

1. Expense Management
2. Attendance Management
3. Grading System
4. Billing System
5. View All Reports
6. Exit

The user selects an option to access the required module.

7. Module Descriptions

7.1 Expense Management

This module manages daily expense records.

Features:

- Add new expenses.
- Enter expense descriptions and amounts.
- Select expense categories.
- View all expense records.
- Calculate category-wise totals.
- Calculate grand total expenses.
- Find the highest and lowest expenses.

Available Categories:

- Food
- Travel
- Utilities
- Stationery
- Other

Validation:

- Description cannot be empty.
- Category must be selected from the available categories.
- Expense amount must be greater than zero.

7.2 Attendance Management

This module maintains attendance records and calculates attendance percentages.

Features:

- Enter total working days.
- Enter student name, roll number and ID.
- Enter present days.
- Calculate attendance percentage.
- Display attendance status.
- Display attendance summary.
- Find highest and lowest attendance.

Formula:

Attendance Percentage = (Present Days / Total Working Days) × 100

Attendance Status:

Percentage| Status
75% or above| Eligible
60% to below 75%| Warning
Below 60%| Shortage

Validation:

- Total working days must be at least 1.
- Present days cannot exceed total working days.
- Roll number cannot be empty or duplicated.

7.3 Student Grading System

This module calculates student performance based on subject marks.

Features:

- Ask the number of students first.
- Enter the number of subjects.
- Enter student names and roll numbers.
- Enter subject-wise marks.
- Calculate total marks.
- Calculate percentage and grade.
- Display PASS or FAIL.
- Generate individual report cards.
- Display class summary and topper details.

Grade Criteria:

Percentage| Grade
90 and above| A+
80–89.99| A
70–79.99| B
60–69.99| C
50–59.99| D
35–49.99| E
Below 35| F

A student fails if any subject has marks below 35.

Validation:

- Number of students must be greater than zero.
- Number of subjects must be greater than zero.
- Marks must be numeric.
- Marks must be between 0 and 100.
- Roll numbers must be unique.

7.4 Billing System

This module generates invoices for customers.

Features:

- Enter customer name.
- Add multiple items.
- Enter item price and quantity.
- Calculate item-wise totals.
- Calculate subtotal.
- Apply discounts.
- Calculate 18% tax.
- Generate the final invoice.

Formulas:

Line Total = Unit Price × Quantity

Taxable Amount = Subtotal − Discount

Tax = Taxable Amount × 18%

Grand Total = Taxable Amount + Tax

Discount Criteria:

Subtotal| Discount
10,000 or above| 15%
5,000 to below 10,000| 10%
1,000 to below 5,000| 5%
Below 1,000| No discount

Validation:

- Customer name cannot be empty.
- Item name cannot be empty.
- Unit price must be greater than zero.
- Quantity must be at least one.
- Invoice is not generated when no items are entered.

7.5 Reports Module

The Reports module combines information from all four modules.

It displays:

1. Expense Report – expense details, category-wise totals and grand total.
2. Attendance Report – student attendance and average attendance.
3. Grading Report – student marks, grades, class average, pass count, fail count and topper.
4. Billing Report – invoice details, subtotal, discount, tax and grand total.

If no records are available, the system displays an appropriate message.

8. Input Validation Module

The validators.py file contains reusable validation functions.

Function| Purpose
get_int()| Accepts valid whole numbers within specified limits.
get_float()| Accepts valid decimal numbers within specified limits.
get_name()| Checks that the entered name is not empty.
get_yes_no()| Accepts yes/no or y/n responses.

These functions reduce repeated validation code and improve the reliability of the application.

9. How to Run the Project

Requirements:

- Python 3 installed.
- PyCharm or another Python IDE.

Execution Steps:

1. Open PyCharm.
2. Open the project folder.
3. Make sure all Python files are in the same folder.
4. Open main.py.
5. Click the Run button.

Alternatively, execute the following command in the terminal:

python main.py

The main menu will appear, and the user can select the required module.

10. Testing Requirements

The application is tested using 20 test cases.

- 12 Normal Test Cases
- 8 Edge Test Cases

Testing covers all four modules, menu navigation, input validation, boundary values and report generation.

The test cases include:

- Valid and invalid menu choices.
- Expense amount validation.
- Attendance percentage calculations.
- Attendance boundary conditions.
- Student grade calculations.
- Invalid and out-of-range marks.
- Billing calculations and discounts.
- Invalid quantity.
- Empty invoice generation.
- Reports with no records.
- Program interruption using Ctrl+C.

The expected results are documented in the separate test file.

11. Expected Output

After successful execution, the system allows users to:

- Manage expense records.
- Maintain attendance records.
- Calculate student grades.
- Generate customer invoices.
- View combined reports.
- Handle invalid inputs through validation functions.

12. Conclusion

The Expense, Attendance, Grading & Billing Management System demonstrates the practical implementation of Python programming concepts.

It provides an organised way to manage different activities through separate modules connected by a common main menu.

This project improves understanding of modular programming, data handling, calculations, input validation and software testing.
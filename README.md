# SmartBudgetManager
A project for managing Budget.
Software Requirements – SmartBudget Manager
Version 1.0 · SmartBudget_Manager.xlsx
1. Document purpose
This document describes what the SmartBudget Manager workbook must do and the conditions under which it must work. It is intended for the developers, testers and technical writers of the product.
2. Product overview
SmartBudget Manager is an Excel workbook that helps users record monthly income and expenses, categorize expenses, calculate the balance automatically, view expenses by category in a chart, and receive a warning when the budget limit is exceeded. It contains three worksheets: Dashboard (balance, totals, charts), Transactions (data entry) and Categories (predefined list: Food, Transport, Rent, Health, Education).
3. Target users
Beginner to intermediate Excel users: individuals, students, families and small-business staff who need a simple budget tracker without learning formulas.
4. Functional requirements
ID	Requirement
FR1	The user shall record income transactions (date, description, amount) in the Transactions sheet.
FR2	The user shall record expense transactions (date, description, category, amount).
FR3	The user shall select the expense category from a dropdown list fed by the Categories sheet.
FR4	The workbook shall calculate total income and total expenses with SUM().
FR5	The workbook shall calculate expenses per category with SUMIF()/SUMIFS().
FR6	The workbook shall calculate the monthly balance (income − expenses) automatically.
FR7	The Dashboard shall display a pie or column chart of expenses by category.
FR8	The user shall set a monthly budget limit; conditional formatting shall highlight overspending when expenses exceed it.
5. Non-functional requirements
    • Performance: Dashboard updates within 1 second of data entry.
    • Usability: clear labels, consistent colours, no formula knowledge needed.
    • Reliability: formulas on the Dashboard are protected; dropdown prevents invalid categories.
    • Compatibility: works in Excel 2016, 2019, 2021 and Microsoft 365.
    • Security: file saved as .xlsx; no macros, so no security warnings.
6. Assumptions and limitations
    • Users have Excel installed and basic keyboard/mouse skills.
    • One workbook covers one month at a time; a yearly view is not included.
    • Single currency, single user; no bank import and no mobile-specific interface.
    • Chart and formulas depend on the Transactions table keeping its structure.

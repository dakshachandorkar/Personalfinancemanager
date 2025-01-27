# Personalfinancemanager
The Personal Finance Manager is a system designed to help users manage their income, expenses, and savings goals effectively. It allows users to track their financial transactions, categorize them, set savings goals, and generate insightful reports to understand their spending patterns.

Features

User Management:
Register and login functionality.
Each user has a unique profile with personal details.

Transaction Management:
Add, view, update, and delete financial transactions.
Transactions include details such as amount, date, category, and description.

Category Management:
Create custom categories for transactions.
View and manage existing categories.

Savings Goals:
Set savings goals with a target amount and date.
Track progress towards these goals.

Report Generation:
Generate monthly and yearly reports showing income, expenses, and savings.
Visual representations of spending categories using Matplotlib.

Data Persistence:
All data is stored in an SQLite database.

Assumptions
Basic authentication is implemented using a username and password.
The application uses SQLite for data storage.
A simple command-line interface (CLI) is provided for user interaction.

Setup Instructions
Prerequisites
Python 3.7 or higher
SQLite3 (usually included with Python)
Matplotlib library

Steps to Run
Clone or download the repository.
Open the project folder in Google Colab or any Python IDE.
Ensure the following Python libraries are installed:
pip install matplotlib

Run the Python script:
python finance_manager.py
Follow the on-screen instructions to register, login, and manage your finances.

Using Google Colab
Upload the script to your Google Drive.
Open it in Google Colab.
Execute each code block sequentially.

Design Overview
The system is designed using object-oriented principles with the following key classes:
UserManager: Handles user registration and login.
TransactionManager: Manages financial transactions.
CategoryManager: Manages custom categories.
SavingsGoalManager: Manages savings goals.
ReportGenerator: Generates reports with visualizations.

Database Schema

Users Table:
id, name, email, password

Transactions Table:
id, user_id, amount, date, category, description

Categories Table:
id, user_id, name

Savings Goals Table:
id, user_id, target_amount, target_date

Testing
Sample Test Cases:

Test Case 1: User Registration
Input: Name: "Emily", Email: "emily@mail.com", Password: "123"
Expected Output: "User registered successfully!"

Test Case 2: User Login
Input: Email: "emily@gmail.com", Password: "123"
Expected Output: "Login successful!"

Test Case 3: Add Transaction
Input: Amount: 100.0, Date: "2025-01-01", Category: "Food", Description: "Lunch"
Expected Output: "Transaction added successfully!"

Test Case 4: Add Category
Input: Category Name: "Utilities"
Expected Output: "Category added successfully!"

Test Case 5: Add Savings Goal
Input: Target Amount: 5000.0, Target Date: "2025-12-31"
Expected Output: "Savings goal added successfully!"

Test Case 6: Generate Report
Input: Generate spending report.
Expected Output: A pie chart displaying spending by category.

Instructions to Run Tests
Run the script as described in the setup instructions.
Follow the menu options to perform each operation.
Verify the outputs against the expected results for each test case.
For visualizations, ensure Matplotlib is installed and working correctly.

Sample Usage
Register as a new user.
Login with your credentials.
Add transactions and categorize them.
Set savings goals and monitor progress.
Generate a report to visualize your spending.


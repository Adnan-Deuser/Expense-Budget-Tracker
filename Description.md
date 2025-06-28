# 💰 Expense & Budget Tracker

## 1. Project Overview

The **Expense & Budget Tracker** is a GUI-based personal finance tool developed in Python using Tkinter. Its core purpose is to help users:

- Log daily expenses
- Set and manage monthly budgets
- Analyze spending patterns through reports and visual charts

By storing data locally in a CSV file and providing a clean, interactive interface, this app simplifies day-to-day money management for users of all technical levels.

## 2. Key Features

| Feature                   | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| 💵 Add Daily Expense       | Input amount, category (e.g., Food, Travel), and optional notes              |
| 🧾 Monthly Budget          | Set a monthly budget and track remaining balance                            |
| 📊 View Reports            | See total spending, remaining budget, and a breakdown by category           |
| 📈 Pie Chart Visualization | Generate category-wise expense charts using Matplotlib                      |
| 💾 Persistent Storage      | Expense data is saved in a local `data.csv` file                            |

## 3. Technologies Used

| Technology   | Purpose                                         |
|--------------|-------------------------------------------------|
| Python 3.x   | Core programming language                        |
| Tkinter      | GUI framework to create forms and buttons        |
| CSV          | Lightweight, file-based expense storage          |
| Matplotlib   | Generate visual pie charts                       |
| Datetime     | Automatically records the date for each entry    |


## 4. Architectural Highlights & Design Choice
### 🖼 GUI-Centric Design
- Tkinter chosen for simplicity and built-in availability in Python.
- Designed for **non-technical users**—no terminal or CLI interaction needed.

### 📂 File-Based Data Storage
- CSV used instead of SQL/NoSQL to keep the app lightweight and dependency-free.
- Automatically timestamps entries for future filtering.

### 🧩 Modular Functional Layout
- Code is structured with clear method separation:
  - `add_expense()`, `view_report()`, `show_chart()`
- GUI and logic components are kept cleanly divided.

### 📊 Visual Reporting
- Matplotlib provides a clear, visual summary of spending habits.
- Pie charts enable users to quickly interpret expense distribution.

## 5. Challenges and Solutions

| Challenge                          | Solution                                                         |
|-----------------------------------|------------------------------------------------------------------|
| Input validation                  | `try-except` blocks with `messagebox` to catch invalid inputs     |
| Avoiding UI clutter               | Used `grid()` layout with appropriate spacing and alignment       |
| Data storage without a database   | Chose structured CSV format for simplicity and readability        |
| Missing data file on first run    | App checks and auto-creates `data.csv` if not found               |
| Incomplete input from user        | Added required field checks and input validation                  |

## 6. Future Enhancements

| Improvement            | Description                                                           |
|------------------------|-----------------------------------------------------------------------|
| 👤 User Accounts        | Add login system to support multiple users                           |
| 🗃 Switch to a Database | Migrate from CSV to SQLite or MongoDB for better scalability         |
| 📆 Date Filtering       | Allow filtering by week, month, or custom date range                 |
| 📤 Export Reports       | Export expense reports as PDF or Excel files                         |
| 🌐 Web Version          | Rebuild the app using Flask or Django for online accessibility       |
| 📱 Mobile App           | Develop an Android version using Kivy or React Native                |

---

Designed with clarity, simplicity, and usability in mind — this project is ideal for beginners and practical enough for daily use.

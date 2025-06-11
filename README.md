# 💰 Personal Expense Tracker – Python Tkinter & MySQL

A user-friendly **Personal Expense Tracker** application built with **Python (Tkinter GUI)** and **MySQL database**. It allows users to track income and expenses, visualize spending, and export detailed reports.

---

## 🔧 Features

- ✅ **User Registration & Login**
  - Create an account using your name, email, and password
  - Email format validation using regex
  - Login to access your personal data
  - Forgot password support

- 💼 **Income Tracking**
  - Add or update your monthly income
  - Income is linked to the logged-in user

- 🧾 **Expense Tracking**
  - Add expenses with category, date, and amount
  - Update or delete past expenses
  - View all your expenses in a table format

- 📊 **Visual Reports**
  - View a **bar chart** of your monthly expenses
  - Generate a **pie chart** showing expense distribution by category

- 📤 **Exporting Reports**
  - Export all your expenses to a **CSV file**
  - Generate a professional-looking **PDF report** of your expenses

---

## 🖥️ Technologies Used

| Technology | Purpose                         |
|------------|----------------------------------|
| Tkinter    | Graphical User Interface (GUI)   |
| MySQL      | Database to store user data      |
| Matplotlib | Bar & Pie chart visualization    |
| FPDF       | PDF report generation            |
| CSV        | Data export                      |
| Regex      | Email format validation          |

---

## 🚀 How It Works

1. **User Login System**
   - User enters email and password
   - If valid, they're redirected to the dashboard
   - If new user, they can register via the signup screen

2. **Add Income**
   - User adds or updates monthly income from the income section
   - Stored in MySQL linked to user’s email

3. **Add Expense**
   - User selects a category, date, and amount
   - Expense is saved and displayed in a table
   - Options to delete or update existing entries

4. **View Charts**
   - Clicking "Bar Graph" or "Pie Chart" generates visual summary using `matplotlib`

5. **Export Data**
   - "Export CSV" saves all expense data to a local CSV file
   - "Generate PDF" creates a downloadable PDF report

---

## ⚙️ Installation Instructions

###  📦 Install Dependencies
Make sure Python is installed (>=3.7), then run:

pip install matplotlib mysql-connector-python fpdf


Set Up MySQL Database
Open MySQL and create a database (e.g., expense_db)

Create a table for user data and expenses as per the structure used in the script

Update the database credentials in the script:

python
Copy
Edit
mydb = mysql.connector.connect(
    host="localhost",
    user="your_username",
    password="your_password",
    database="expense_db"
)


# 💰 Expense Tracker Web App

This project is a **full-stack Expense Tracker** built using **Django**, **MySQL**, and **HTML/CSS/JavaScript**. It allows users to securely manage and track their personal or business expenses in real-time via a web interface.
## 🎯 Objective
To build a responsive and feature-rich application that allows users to:
- Log income and expenses
- Categorize transactions (e.g., Food, Travel, Bills, Shopping)
- Track balance, spending trends, and financial summaries
- View interactive charts and downloadable reports

---

## ⚙️ Tech Stack

- **Frontend**: HTML, CSS, Bootstrap, JavaScript
- **Backend**: Django (Python)
- **Database**: MySQL
- **Charting**: Chart.js or Plotly (optional)
- **Authentication**: Django's built-in auth system

---

## 📁 Features

### ✅ User Authentication
- Register / Login / Logout
- Password hashing and session management

### ✅ Expense Management
- Add income/expense transactions with date, description, amount, and category
- Edit or delete past entries

### ✅ Dashboard
- Display total balance, income, and expenses
- Show recent transactions
- Visualizations of category-wise spending (pie/bar charts)
- Monthly summary

### ✅ Filtering & Reports
- Filter transactions by date, category, or type
- Export filtered reports to CSV

---

## 🚀 How to Run Locally

### 1. Clone the repository
git clone https://github.com/your-username/django-expense-tracker.git
cd django-expense-tracker
### 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
### 3. Install dependencies
pip install -r requirements.txt
### 4. Configure your MySQL database
- Create a MySQL database (e.g., `expense_db`)
- Update `DATABASES` section in `settings.py`:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'expense_db',
        'USER': 'your_mysql_user',
        'PASSWORD': 'your_mysql_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### 5. Run migrations
python manage.py makemigrations
python manage.py migrate
### 6. Run the server
python manage.py runserver
Visit `http://127.0.0.1:8000` in your browser to access the app.
## 🧩 Folder Structure
📁 django-expense-tracker
├── expense_tracker/               # Main Django app
├── templates/                     # HTML templates
├── static/                        # CSS, JS, and static files
├── db.sqlite3 / mysql setup       # Database
├── manage.py                      # Django management script
├── requirements.txt               # Project dependencies
└── README.md                      # Project documentation
## 🔐 Security Notes
- CSRF protection is enabled by default in Django.
- All user data is stored securely and isolated per session.
- Never expose sensitive data like passwords or API keys.
## 📄 License
MIT License – feel free to use, modify, and distribute with credit.
## 🙋 Author
- Sai Teja Vinukonda
- GitHub: https://github.com/SaitejaVinukonda

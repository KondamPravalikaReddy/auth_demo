🔐 Multi-User Authentication Demo (Flask)

A production-style multi-user authentication system built with Python (Flask).
This project demonstrates secure signup, login, session-based authentication, and personalized dashboards, following industry best practices.

✨ Features

Secure user signup with validation

Password hashing using bcrypt

Login with session management

CSRF protection on all forms

Personalized dashboards per user

Secure logout with session invalidation

SQLite database (no external setup required)

🧱 Tech Stack
Backend

Python 3.10+

Flask

Flask-Login

Flask-WTF

Flask-SQLAlchemy

bcrypt

Frontend

HTML (Jinja2 templates)

CSS

Database

SQLite

📁 Project Structure
auth_demo/
├── app.py              # Main Flask application
├── models.py           # Database models
├── forms.py            # Form validation & CSRF
├── requirements.txt    # Dependencies
│
├── templates/
│   ├── signup.html
│   ├── login.html
│   └── dashboard.html
│
├── static/
│   └── styles.css
│
└── README.md

▶️ Running the Project Locally
1️⃣ Create a Virtual Environment
python -m venv venv


Activate it:

macOS / Linux

source venv/bin/activate


Windows

venv\Scripts\activate

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run the Application
python app.py

4️⃣ Open in Browser
http://127.0.0.1:5000

🔄 Authentication Flow
📝 Signup

User submits email and password

Inputs validated on the server

Password hashed using bcrypt

User stored securely in the database

🔑 Login

Credentials verified

Session created using Flask-Login

User redirected to dashboard

📊 Dashboard

Accessible only when authenticated

Displays logged-in user’s email

Sessions are isolated per user

🚪 Logout

Session destroyed

Authentication cookie invalidated

User redirected to login page

🔒 Security Measures

Password hashing with bcrypt

CSRF protection on all forms

Server-side input validation

No account enumeration in error messages

Secure session cookies

Protected routes using @login_required

⚠️ Edge Cases Handled

Duplicate email registration

Invalid login credentials

Expired sessions

Concurrent logins from different devices

Unauthorized dashboard access

🚀 Intended Use

This project is suitable for:

Authentication demos

Learning secure Flask authentication patterns

MVPs and internal tools

Portfolio or interview projects

🔧 Optional Enhancements

Possible extensions:

JWT-based API authentication

Password reset flow

Email verification

Rate limiting / brute-force protection

Role-based access control

Dockerized deployment

📜 License

This project is provided for educational and demonstration purposes.
You are free to modify and use it as needed.
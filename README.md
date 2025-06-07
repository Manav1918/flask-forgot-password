# 🔐 Flask Forgot Password Feature - Tutorial App

This project demonstrates how to implement a secure **Forgot Password** functionality in a Flask web application, along with user **Registration**, **Login**, **Change Password**, and **Reset Password** workflows.

---

## 🚀 Features

- User Registration
- User Login and Logout
- Forgot Password (via Email Reset Link)
- Change Password
- Password Hashing for security
- Email Integration for sending password reset links
- Flash messages and validation feedback
- Responsive and user-friendly UI (optional Bootstrap support)

---

## 📁 Folder Structure

```
project/
│
├── app.py                 # Main Flask app
├── templates/             # HTML templates (Jinja2)
│   ├── login.html
│   ├── home.html
│   ├── form_models.html
│   ├── reset_password.html
│   └── base.html
├── static/                # Static files (CSS, JS, images)
├── test1.sql             # Database file for illustration. Create 'test1' named database and import this sql for creating 'usertable' used in this app.
└── requirements.txt       # Python dependencies
```

---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/flask-forgot-password.git
   cd flask-forgot-password
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   venv\Scripts\activate   # On Windows
   source venv/bin/activate  # On macOS/Linux
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure email settings**  
   In `mailSetup()` method in app.py, set your email data:
   ```python
   MAIL_SERVER = 'smtp.yourprovider.com'
   MAIL_PORT = 587
   MAIL_USE_TLS = True
   MAIL_USERNAME = 'your-email@example.com'
   MAIL_PASSWORD = 'your-app-password'
   SECRET_KEY = 'your-secret-key'
   ```

---

## ▶️ Running the App

```bash
python app.py
```

Then open your browser at: [http://localhost:5000](http://localhost:5000)

---

## 📧 Forgot Password Workflow

1. User Enters registered email.
2. clicks "Forgot Password".
3. Receives a link via email.
4. User clicks link to reset password.
5. A reset password page opens which is valid for 1 hour only.
6. User enters new password
7. Password successfully updated.

---

## 🧰 Built With

- Python 3.x
- Flask
- Flask-Mail
- Flask-WTF (optional)
- SQLite (or any database)
- HTML/CSS

---

## 📹 Tutorial

This app is explained step-by-step in the video tutorial:  
👉 [Watch on YouTube](https://your-youtube-link.com)

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙏 Acknowledgements

Thanks for watching and supporting the channel.  
Made with ❤️ by [CID An Education Hub].

# 🔗 URL Shortener

A lightweight and efficient **Flask-based URL Shortener** that allows users to easily shorten long URLs, manage them, and redirect to the original links.  
Built using **Python**, **Flask**, and **SQLite**, this project demonstrates clean backend design, database handling, and basic frontend templating.

---

## 🚀 Features

- ✂️ Shorten long URLs into compact shareable links
- 🔁 Automatic redirection to the original URL
- 💾 Persistent storage using SQLite database
- 📊 Click analytics (track how many times each link was used)
- ⚠️ Custom 404 error page for invalid links
- 🧩 Modular project structure with templates and models
- 🔐 Environment-isolated setup using `venv`

---

## 🛠️ Tech Stack

| Layer           | Technology              |
| --------------- | ----------------------- |
| **Backend**     | Python (Flask)          |
| **Database**    | SQLite                  |
| **Frontend**    | HTML5, Jinja2 templates |
| **Environment** | Virtualenv (venv)       |

---

## 📁 Project Structure

```
url_shortener/
├── app.py                 # Main Flask app
├── models.py              # Database models
├── database.db            # SQLite database (auto-created)
├── templates/
│   ├── index.html         # Main homepage
│   └── 404.html           # Error page
├── requirements.txt       # Python dependencies
├── venv/                  # Virtual environment (excluded in .gitignore)
└── README.md              # Project documentation
```

---

## ⚙️ Installation & Setup

Follow these steps to set up and run the project locally 👇

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/url_shortener.git
cd url_shortener
```

### 2️⃣ Create a Virtual Environment

```bash
python -m venv venv
```

### 3️⃣ Activate the Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Mac/Linux:**

```bash
source venv/bin/activate
```

### 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 5️⃣ Run the Application

```bash
python app.py
```

The app will start on:  
👉 **http://127.0.0.1:5000/**

---

## 🧠 How It Works

1. User submits a long URL through the web interface.
2. Flask backend generates a short unique key.
3. The key and original URL are stored in SQLite (`database.db`).
4. When someone visits the short link (e.g., `/abc123`), the app redirects to the original URL.
5. If a key doesn't exist, a custom 404 error page is displayed.

---

## 🧩 Example

**Input:**

```
https://www.example.com/this-is-a-very-long-url
```

**Output:**

```
http://127.0.0.1:5000/abc123
```

Visiting the shortened link automatically redirects to the original site.

---

## 🤝 Contributing

Pull requests are welcome!  
If you'd like to suggest improvements or add features, fork the repo and submit a PR.

---

⭐ **If you like this project, don't forget to give it a star on GitHub!**

# Django To‑Do List (Educational Project)

A tiny Django app built for learning purposes: create lists, add items, check/uncheck them, and save the state. This repo is meant to demonstrate basic Django patterns (views, models, forms, templates)
I created this site to teach basics of Django.

---

## ✨ Features

* Create multiple to‑do lists
* Add, check, and uncheck items
* Persist state in a SQLite database (default)
* Basic Django templating and CSRF protection
* Clear, minimal code for beginners to read and modify

---

## 🎯 Purpose

This project exists **for educational purposes only**. Feel free to fork it, experiment, and break things—then fix them! It’s a great sandbox to practice Django, HTML forms, and version control with Git.

---

## 🧰 Tech Stack

* **Python** ≥ 3.10
* **Django** (see `requirements.txt`)
* **SQLite** (default local DB)
* **HTML/CSS** with Django templates

---

## 🚀 Getting Started

### 1. Get the code onto your machine

Download or copy the project folder into your workspace (e.g., VS Code).

### 2. Create & activate a virtual environment

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```


### 4. Apply migrations & run the server

```bash
python manage.py migrate
python manage.py runserver
```

Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

---

## 🛠 Project Structure (simplified)

```
📁 project_root/
├── main/              # Your main Django app
│   ├── views.py
│   ├── models.py
│   ├── forms.py
│   └── ...
├── templates/
│   ├── base.html
│   ├── home.html
│   ├── list.html
│   ├── create.html
│   └── ...
├── mysite/          # Project root and Django project config (settings, urls, wsgi)
├── manage.py        
├── requirements.txt
└── README.md
```

---

## ✅ Usage

1. Go to the homepage and create a new list.
2. Add items to your list.
3. Check/uncheck items and click **Save** to persist changes.

If you run into issues with checkboxes not saving, confirm that:

* Template checkbox names match what the view expects
* You handle unchecked boxes (they don't show up in POST)


---

## 🌐 (Optional) Deploy

If you want this live on the internet (not just on localhost):

* **Render / Railway / Fly.io / Koyeb / Deta**: connect your GitHub repo and they auto-deploy.
* Add a `Procfile` (for Gunicorn) and configure environment variables (SECRET\_KEY, DEBUG, DATABASE\_URL, etc.).

Example `Procfile`:

```
web: gunicorn project_root.wsgi
```

---

## 🧪 Tests (Optional)

Add unit tests in `tests.py` and run:

```bash
python manage.py test
```

---

## 🤝 Contributing

PRs are welcome! Keep it beginner-friendly:

* Comment your code
* Follow Django best practices
* Update this README when you add features


---

## 📚 Resources

* [Django Official Docs](https://docs.djangoproject.com/)
* [Git Official Docs](https://git-scm.com/doc)
* [VS Code Python](https://code.visualstudio.com/docs/python/python-tutorial)

---

## TODO / Roadmap (Ideas)

* Add user authentication
* Add due dates & categories for items
* Add search/filter functionality
* Add API endpoints (Django REST Framework)
* Add tests & CI (GitHub Actions)

---
My name is Mahdi
Happy coding! 🚀


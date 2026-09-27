# Task Manager

A Django to-do app where signed-in users can create, track and complete tasks.

## Features

- 🔐 Login and logout with Django's built-in authentication
- ✅ Create, view, edit and delete tasks
- Mark tasks as completed
- 🛡️ All views protected with `@login_required`
- ModelForms for validated input

## Tech Stack

**Backend:** Python, Django
**Frontend:** Django Templates, HTML
**Database:** SQLite

## Getting Started

```bash
git clone https://github.com/luka357/taskmanager.git
cd taskmanager
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install django
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Open http://127.0.0.1:8000/login/ and sign in. You'll be taken to `/tasks/`.

## Routes

| URL | Description |
|---|---|
| `/login/`, `/logout/` | Authentication |
| `/tasks/` | Task list |
| `/tasks/add/` | Create a task |
| `/tasks/<id>/` | Task details |
| `/tasks/<id>/update/` | Edit a task |
| `/tasks/<id>/delete/` | Delete a task |

## Project Structure

- `core/` — project settings and root URLs
- `tasks/` — `Task` model, form, views and templates
- `templates/registration/` — login page

## Author

**Luka Julakidze**
[LinkedIn](https://www.linkedin.com/in/luka-julakidze) · [GitHub](https://github.com/luka357)

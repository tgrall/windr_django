# Windr Django App

This is a Django web application project.

## Setup

1. **Activate the virtual environment:**
   ```bash
   source .venv/bin/activate
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run migrations:**
   ```bash
   python manage.py migrate
   ```

4. **Start the development server:**
   ```bash
   python manage.py runserver
   ```

   The application will be available at http://127.0.0.1:8000/

## Project Structure

- `windr_app/` - Main Django project directory
  - `settings.py` - Django settings
  - `urls.py` - URL routing
  - `wsgi.py` - WSGI configuration
  - `asgi.py` - ASGI configuration
- `manage.py` - Django management script
- `requirements.txt` - Python dependencies
- `db.sqlite3` - SQLite database (created after first migration)

## Creating Apps

To create a new Django app:
```bash
python manage.py startapp app_name
```

## Admin Interface

To create a superuser for the admin interface:
```bash
python manage.py createsuperuser
```

Then visit http://127.0.0.1:8000/admin/

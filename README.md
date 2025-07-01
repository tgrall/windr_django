# Windr Django App

This is a Django web application project.

**Repository:** [tgrall/windr_django](https://github.com/tgrall/windr_django)

## Setup

### Initial Setup (Already Done)
The project has been initialized with:
- Django project structure
- Virtual environment with dependencies
- Git repository with initial commit

### Development Setup

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

## Git Workflow

The project is already initialized with Git. For ongoing development:

```bash
# Check status
git status

# Add changes
git add .

# Commit changes
git commit -m "Your commit message"

# View commit history
git log --oneline
```

### Connecting to GitHub

After creating the repository on GitHub (tgrall/windr_django), connect your local repository:

```bash
# Add the remote repository
git remote add origin https://github.com/tgrall/windr_django.git

# Push your code to GitHub
git branch -M main
git push -u origin main
```

### Cloning the Repository

If someone else wants to work on this project:

```bash
# Clone the repository
git clone https://github.com/tgrall/windr_django.git
cd windr_django

# Set up the virtual environment
python -m venv .venv
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate
```

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

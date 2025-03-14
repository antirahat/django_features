# django_features

This repository contains my Django exercise codes. It includes various Django features and functionalities that I've implemented for learning and practice purposes.

## Project Structure

```
demo/
  ├── demo/           # Project configuration directory
  │   ├── settings.py # Django settings
  │   ├── urls.py     # Project URL configuration
  │   └── wsgi.py     # WSGI configuration
  ├── myapp/          # Main application directory
  │   ├── models.py   # Database models
  │   ├── views.py    # View functions
  │   ├── urls.py     # App URL configuration
  │   ├── admin.py    # Admin interface setup
  │   └── templates/  # HTML templates
  ├── manage.py       # Django management script
  └── db.sqlite3      # SQLite database
```

## Setup Instructions

1. Clone the repository
2. Create a virtual environment (recommended)
3. Install dependencies
4. Run migrations: `python manage.py migrate`
5. Create a superuser: `python manage.py createsuperuser`
6. Start the development server: `python manage.py runserver`

## Current Features

### Todo List Application
- Basic CRUD operations for managing todo items
- Model structure:
  ```python
  class TodoItem(models.Model):
      title = models.CharField(max_length=200)
      completed = models.BooleanField(default=False)
  ```
- Features:
  - Create, read, update, and delete todo items
  - Mark todos as completed/incomplete
  - Admin interface integration for easy management
  - Template-based UI for todo list display

### Views
- Home page view
- Todo list display view with all todo items

### Admin Interface
- Integrated Django admin interface
- TodoItem model registered for admin management
- Easy CRUD operations through admin panel
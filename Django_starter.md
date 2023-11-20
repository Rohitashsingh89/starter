# Django Starter Kit

This is a simple guide to help you set up a basic Django project.

## Prerequisites

Make sure you have the following installed on your machine:

- [Python](https://www.python.org/)
- [pip](https://pip.pypa.io/en/stable/)

## Create a new Django project

Open your terminal and run the following commands:

```bash
# Create a virtual environment (optional but recommended)
python -m venv myenv
source myenv/bin/activate  # On Windows, use `myenv\Scripts\activate`
```

# Install Django
```bash
pip install django
```

# Create a new Django project
```bash
django-admin startproject myproject
cd myproject
```

This will create a new Django project in a folder called `myproject` and navigate into that folder.

## Run the development server

Inside your project folder, run:

```bash
python manage.py runserver
```

This will start the development server, and you can access your Django app at [http://localhost:8000](http://localhost:8000).

## Create a superuser

To create a superuser (admin) account, run the following command:

```bash
python manage.py createsuperuser
```

Follow the prompts to enter a username, email address, and password for the superuser.

## Create an django app 

To create a app in django, run the following command:

```bash
python manage.py startapp myapp
```
This will create a app in your django project.

## Project Structure

The basic project structure will look like this:

```
myproject/
|-- manage.py
|-- myproject/
|   |-- __init__.py
|   |-- asgi.py
|   |-- settings.py
|   |-- urls.py
|   |-- wsgi.py
|-- myapp/
|   |-- __init__.py
|   |-- admin.py
|   |-- apps.py
|   |-- migrations/
|   |-- models.py
|   |-- tests.py
|   |-- views.py
|-- myenv/  # Virtual environment folder (if created)
|-- db.sqlite3
```

- `manage.py`: Django command-line utility.
- `myproject/`: Main project folder.
- `myapp/`: app folder.

## Additional Setup

You might want to explore other tools and libraries to enhance your Django development experience:

- [Django REST framework](https://www.django-rest-framework.org/): For building APIs with Django.
- [Django ORM](https://docs.djangoproject.com/en/3.2/topics/db/models/): Object-Relational Mapping for database interactions.
- [Django Templates](https://docs.djangoproject.com/en/3.2/topics/templates/): For rendering HTML templates.

Happy coding! 🐍

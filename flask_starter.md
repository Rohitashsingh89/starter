# Flask Starter Kit

This is a simple guide to help you set up a basic Flask project.

## Prerequisites

Make sure you have the following installed on your machine:

- [Python](https://www.python.org/)
- [pip](https://pip.pypa.io/en/stable/)

## Create a new Flask project

Open your terminal and run the following commands:

```bash
# Create a new directory for your project
mkdir my-flask-project
cd my-flask-project

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

# Install Flask
pip install Flask
```

This will create a new directory called `my-flask-project`, set up a virtual environment, activate it, and install Flask.

## Create a minimal Flask app

Create a file named `app.py` in your project directory and add the following code:

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
    return 'Hello, Flask!'

if __name__ == '__main__':
    app.run(debug=True)
```

## Run the Flask app

In your terminal, run the following command to start the Flask development server:

```bash
python app.py
```

You can access your Flask app at [http://localhost:5000](http://localhost:5000).

## Project Structure

The basic project structure will look like this:

```
my-flask-project/
|-- venv/  # Virtual environment folder
|-- app.py
|-- README.md
```

- `venv/`: The folder containing the virtual environment (if created).
- `app.py`: The main file where you define your Flask app.

## Additional Setup

You might want to explore other tools and libraries to enhance your Flask development experience:

- [Flask-Restful](https://flask-restful.readthedocs.io/): For building REST APIs with Flask.
- [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/): For working with databases using SQLAlchemy.
- [Jinja2](https://jinja.palletsprojects.com/): Templating engine for rendering HTML templates in Flask.

Happy coding with Flask! 🐍

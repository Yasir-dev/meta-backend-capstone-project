# Meta Backend Capstone final project

This project is a Django backend project for a hypothetical application.


## Configue the Database

Login to the MySQL Database shell and run the following commands

- `create database littlelemon;`
- `use littlelemon;`
- `CREATE USER 'admindjango'@'localhost' IDENTIFIED BY 'password';`
- `GRANT ALL PRIVILEGES ON littlelemon.* TO 'admindjango'@'localhost';`
- `GRANT ALL PRIVILEGES ON `test_littlelemon`.* TO 'django'@'localhost';`
- `FLUSH PRIVILEGES;`

## Installation

- Clone the repository
- Run `pipenv shell` to start your virtual environment.
- Run `pipenv install` to install the required dependencies from the Pipfile.
- Run `python manage.py makemigrations` to create new migrations based on the changes you have made to your models.
- Run `python manage.py migrate` to apply and unapply migrations.
- Run `python manage.py runserver` to start the development server.


## API Endpoints

## URL Configuration

- `/admin/`: This URL is for the Django admin interface.
- `/api/`: This URL is for the API endpoints of the restaurant app.
- `auth/`: This URL is for the authentication endpoints provided by Djoser. Djoser provides a set of Django Rest Framework views to handle basic actions such as registration, login, logout, password reset and account activation. It works with custom user model.

## Run the tests

`python manage.py test`
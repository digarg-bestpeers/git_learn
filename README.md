# Real Estate Management

## Technology Stack
1. Python environment: python 3.5.2
1. Framework: Django = 2.2.11
1. UI Technology: HTML, CSS, BS, JS

## Installation Set Up
* click on [install]("https://pypi.org/project/virtualenv/") to create virtual environment










## Create Database

* sudo -u postgres psql
* CREATE DATABASE real_estatedb;
* \l
* \q

## Instruction

* clone the project
* set Postgresql Database settings in setting.py
```python
            DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'real_estatedb',
        'USER': 'root',
        'PASSWORD': 'root',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}
```
* do migration
```python
           python manage.py makemigrations
           python manage.py migrate
```
* create superuser
```python
         python manage.py createsuperuser
```
* access project
```python
              python manage.py runserver
```




# Real Estate Management

## Feature
1. __Property Module__: reflect all available property

## Technology Stack
1. Python environment: python 3.5.2
1. Framework: Django = 2.2.11
1. UI Technology: HTML, CSS, BS, JS

## Installation Set Up
* click on [install](https://pypi.org/project/virtualenv/) to create virtual environment
* install python 3.5
```python
            sudo apt-get install python3.5
```
* install requirement.txt for all project dependencies
* install postgresql database
```batch
            sudo apt-get install postgresql postgresql-contrib
```

## Create Database

* sudo -u postgres psql
* CREATE DATABASE real_estatedb;
* \l
* \q

## How to use

1. clone the project
1. update settings.py file 
```python
# Database Configration
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
3. Use following commands to migrate the table
```python
           python manage.py makemigrations
           python manage.py migrate
```
4. Then start the project directly with following command
```python
              python manage.py runserver
```




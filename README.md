# Real Estate Management

## Create and Activate Virtual Environment

```bash
      pip install virtualenv
      virtualenv env_name
      . env_name/bin/activate
```

## Install Python and django

```bash
     pip install python 3.5
     pip install django = 2.2.11
```

## Install pillow package

```bash
        pip install pillow
```

## Install Postgresql Database

```bash
        sudo apt-get install postgresql postgresql-contrib
```

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




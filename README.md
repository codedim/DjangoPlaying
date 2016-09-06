# DjangoPlaying

This is just a practice repository -- a "Hello world!" project -- to play with 
**Django** framework and **Python** programming language.

#### Links:

 http://tutorial.djangogirls.org/
 http://codedim.pythonanywhere.com/


## Part 1. Start Django Web-Server

> Note: You need to have installed **Python3** and **Git** applications before.
>       The following information is intended for Windows platforms basically.


#### Install Django

```
 > mkdir django
 > cd django
 > python3 -m venv myvenv
 > myvenv\Scripts\activate
 (myvenv) > pip install django==1.8
 (myvenv) > django-admin startproject mysite .
```

#### Catalogs

```
 django
 |___manage.py
 |___mysite
        settings.py
        urls.py
        wsgi.py
        __init__.py
```

#### Edit mysite\settings.py

```
 TIME_ZONE = 'Europe/Moscow'
 STATIC_URL = '/static/'
 STATIC_ROOT = os.path.join(BASE_DIR, 'static')
```

#### Create DB

```
 (myvenv) > python3 manage.py migrate
```

#### Start the Server

```
 (myvenv) > python3 manage.py runserver
```

#### Check out the home-page

```
 http://localhost:8000/
```


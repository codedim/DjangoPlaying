# Links:

 http://tutorial.djangogirls.org/ru/


# Install Django

 > mkdir django
 > cd django
 > python3 -m venv myvenv
 > myvenv\Scripts\activate
 (myvenv) > pip install django==1.8
 (myvenv) > django-admin startproject mysite .


# Catalogs

 django
 |___manage.py
 |___mysite
        settings.py
        urls.py
        wsgi.py
        __init__.py


# Edit mysite\settings.py

 TIME_ZONE = 'Europe/Moscow'
 STATIC_URL = '/static/'
 STATIC_ROOT = os.path.join(BASE_DIR, 'static')


# Create DB

 (myvenv) > python3 manage.py migrate


# Start the Server

 (myvenv) > python3 manage.py runserver


# Check the home-page

 http://localhost:8000/


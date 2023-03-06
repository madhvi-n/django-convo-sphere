# Django-Convo-Sphere
[![Django CI](https://github.com/madhvi-n/django-convo-sphere/actions/workflows/django.yml/badge.svg)](https://github.com/madhvi-n/django-convo-sphere/actions/workflows/django.yml)

Django-Convo-Sphere is a chat messenger project powered by Django, Celery and Redis. It enables users to create chat rooms, add contacts, and send messages in real-time. The project leverages Redis Pub/Sub for real-time communication, Celery for message processing, and Django's ORM for data management.


# Requirements
- Backend
    - Python 3.8+
    - virtualenv
    - WSL


- Frontend
    - Angular 10.2.4 (or 10.2.5)
    - Node 10.13.x +



# Installation

Clone the repository and enter the root directory
```
git clone https://github.com/madhvi-n/django-convo-sphere.git
cd django-convo-sphere
```


Create a virtual environment and activate it
```
virtualenv venv
source venv/bin/activate
```

Making sure your virtual environment is activated, install the dependencies using `pip`
```
pip install -r requirements.txt
```

You can set the secret key for django project in 2 ways
- Edit the `django_convo_sphere/settings.py` file and add a key manually, some random string.
- Edit the venv file to export `SECRET_KEY`


After installing dependencies, migrate Django apps.(You will find the list of apps when you run the command `python manage.py runserver`)
```
python manage.py migrate
```

Finally start your Django server
```
python manage.py runserver
```

Visit `http://127.0.0.1:8000/` or `localhost:8000` for running web server
Alternatively you can access the admin interface on `http://127.0.0.1:8000/admin/` or `localhost:8000/admin`

Access python shell
```
python manage.py shell
```

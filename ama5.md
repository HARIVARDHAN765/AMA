# AMA

## 1. Adhikya Edammala: What does MVT stand for in Django?

MVT stands for:

* **Model** – Handles database operations.
* **View** – Contains the business logic.
* **Template** – Displays data to the user using HTML.

## 2. Allanki VV Manikanta Sai: Can Django work without a Database?

Yes, Django can work without a database for simple static websites.

## 3. Arpit Yadav: On which ports do HTTP and HTTPS work?


* **HTTP** works on **Port 80**
* **HTTPS** works on **Port 443**


## 4. Boorle Sowmya Sri Lakshmi: What does `settings.py` tell in Django?

**Answer:**

`settings.py` is the main configuration file of a Django project.

It contains:

* Installed apps
* Database settings
* Templates settings
* Static files settings
* Security settings
* Middleware configuration


## 5. Injamuri Arun Kumar: How do you start a Django server?

```bash
python manage.py runserver
```

## 6. Md Musharaf: How do you create a web app in Django?

Create a new app using:

```bash
python manage.py startapp app_name
```
Then add the app name to `INSTALLED_APPS` in `settings.py`.

## 7. Naman Sharma: Why do we use migrations in Django?

**Answer:**

Migrations are used to apply database changes created in models.

They help:

* Create tables
* Modify tables
* Add or remove fields
* Keep the database structure synchronized with models

Commands:

```bash
python manage.py makemigrations
python manage.py migrate
```


## 8. Nayunipatruni Harsha Vardhan: How do you create a project in Django?


Use:

```bash
django-admin startproject project_name
```


## 9. Parlapalli Sulochana: How can we inherit HTML files from one another?

Django uses **Template Inheritance**.

Parent file:

```html
{% block content %}
{% endblock %}
```

Child file:

```html
{% extends "base.html" %}

{% block content %}
<h1>Welcome</h1>
{% endblock %}
```


## 10. Rongala Vasu: What is a Template?

A template is an HTML file that displays data to users.

## 11. Rovinpal Udupi: What does `manage.py` do in Django?


`manage.py` is a command-line utility used to manage a Django project.

Common commands:

```bash
python manage.py runserver
python manage.py migrate
python manage.py createsuperuser
python manage.py shell
```

It helps interact with the Django project.


## 12. Tumma Haritha: What is Latency?

Latency is the time taken for data to travel from the sender to the receiver.

## 13. Vikas Mehta: Difference between `get()` and `filter()` in Django


| get()                          | filter()                             |
| ------------------------------ | ------------------------------------ |
| Returns one object             | Returns a QuerySet                   |
| Raises exception if not found  | Returns empty QuerySet if not found  |
| Used when expecting one record | Used when expecting multiple records |


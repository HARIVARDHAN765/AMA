# AMA

## 1. What is the use of the dotenv library?

The **dotenv** library loads values from a `.env` file into your Django project.

We use it to keep sensitive information like:

* SECRET_KEY
* Database password
* API keys

## 2. What is a Foreign Key?

A **Foreign Key** is used to connect two database tables.

### Example

One User can create many Posts.

So, the Post table stores the User's ID as a Foreign Key.

```python
user = models.ForeignKey(User, on_delete=models.CASCADE)
```

## 3. How do you stop client-side form validation in Django?

Add the `novalidate` attribute to the `<form>` tag.

```html
<form method="POST" novalidate>
```

Now the browser won't validate the form.
Django will validate it on the server.

---

## 4. What does `python manage.py dbshell` do?

It opens your project's database in the terminal.

You can run SQL queries directly.

Example:

```bash
python manage.py dbshell
```

---

## 5. What is Gunicorn?

Gunicorn is a **WSGI server** used to run Django projects in production.

We do **not** use:

```bash
python manage.py runserver
```

in production because it is only for development.

Instead, we use Gunicorn because it is:

* Faster
* More secure
* Can handle many users

---

## 6. What is the Pillow library used for?

Pillow is used to work with images.

It can:

* Upload images
* Resize images
* Crop images
* Rotate images
* Compress images

It is mainly used with Django's `ImageField`.

---

## 7. What does the `authenticate()` method do?

`authenticate()` checks whether the username and password are correct.

If they are correct:

* It returns the User object.

If they are wrong:

* It returns `None`.

It only checks the credentials.
It **does not log the user in**.

---

## 8. Difference between `select_related()` and `prefetch_related()`

### `select_related()`

* Used with **ForeignKey** and **OneToOneField**.
* Fetches related data using one SQL query.
* Makes the query faster.

### `prefetch_related()`

* Used with **ManyToManyField** and reverse ForeignKey.
* Uses separate SQL queries.
* Also improves performance.

---

## 9. Common fields in Django Forms

Some commonly used form fields are:

* `CharField` – Text
* `EmailField` – Email
* `IntegerField` – Numbers
* `BooleanField` – Checkbox
* `ChoiceField` – Dropdown
* `DateField` – Date
* `FileField` – File upload
* `ImageField` – Image upload

---

## 10. What does `login_required` do?

`login_required` allows **only logged-in users** to access a view.

Example:

```python
@login_required
def dashboard(request):
    ...
```

If the user is not logged in, Django sends them to the login page.

---

## 11. What is URL Reversing?

URL reversing means using the **URL name** instead of writing the URL path directly.

Example:

```python
path("profile/", views.profile, name="profile")
```

Instead of writing:

```html
<a href="/profile/">
```

Write:

```html
<a href="{% url 'profile' %}">
```


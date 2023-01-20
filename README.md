# **[Django Admin Atlantis PRO](https://appseed.us/product/atlantis-dark-pro/django/)**

**Django** starter styled with **[Atlantis PRO](https://appseed.us/product/atlantis-dark-pro/django/)**, a premium `Bootstrap 4` design from `ThemeKita`.
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-atlantis-pro`

<br />

## Features: 

- **UI Kit**: Atlantis BS4 PRO `v2.0.1` by ThemeKita
- [Django Atlantis PRO](https://appseed.us/product/atlantis-dark-pro/django/) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Django Atlantis PRO](https://user-images.githubusercontent.com/51070104/212669274-3eef24b4-7c19-4557-99c5-e24ae5b14a5b.png)

<br />

## Why `Django Admin Atlantis PRO`

- Modern [Bootstrap](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

Atlantis Dashboard PRO comes with error/bug-free, well structured codebase that renders nicely in all major browsers and devices. 

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install git+https://github.com/app-generator/priv-django-admin-atlantis-pro.git
```

<br />

> Add `admin_atlantis_pro` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_atlantis_pro.apps.AdminAtlantisProConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_atlantis_pro` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_atlantis_pro.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

## Screenshots

![Django Admin Atlantis PRO - Main Dashboard Page.](https://user-images.githubusercontent.com/51070104/213626540-300ee6e1-f051-449d-be54-0e8c9e07cd99.jpg)

<br />

> [Django Admin Atlantis PRO](https://appseed.us/product/atlantis-dark-pro/django/) - `Maps Page`

![Django Admin Atlantis PRO - Maps Page.](https://user-images.githubusercontent.com/51070104/213626614-0eb12373-f975-406c-a868-058e3cf24df3.jpg)

<br />

> [Django Admin Atlantis PRO](https://appseed.us/product/atlantis-dark-pro/django/) - `Charts Page`

![Django Admin Atlantis PRO - Charts Page.](https://user-images.githubusercontent.com/51070104/213626717-960c4545-bbce-4372-b7c9-09ea1cd5865d.jpg)

<br />

---
**[Django Admin Atlantis PRO](https://appseed.us/product/atlantis-dark-pro/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**

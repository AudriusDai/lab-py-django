# lab-py-django

Experimenting with Python and [Django](https://www.djangoproject.com/) for web development. Checking tutorial series - [Django Web Development with Python](https://www.youtube.com/watch?v=yD0_1DPmfKM&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3). Also the text tutorials - [Django Web Development with Python (text)](https://pythonprogramming.net/admin-apps-django-tutorial/)

## [Introduction](https://www.youtube.com/watch?v=yD0_1DPmfKM&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3)

In video the 2.1.x is used. But I have installed the 3.0.4 .

```
> pip install django
```

Django considers a website to be a collection of apps. (i.e. store app, blog app). Official Django tutorial is [here](https://docs.djangoproject.com/en/3.0/intro/tutorial01/). `(also read Flask vs Django)`

Build -> add sub-site -> run locally.

```
> django-admin startproject crawlers
> py manage.py startapp crawlers_auto
> py manage.py runserver
```

## [Models](https://www.youtube.com/watch?v=aXxIjeGR6po&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=2)

Create/define model -> make migrations -> migrate model. `(model == table)`

If making/updating the model you have to do migrations. But before running the migrations, we have to actually install the `crawlers_auto` app. The initial create operation was not enough. Apparently you have to also do the `install`. Add sub-app into config of core app.

```
> py manage.py makemigrations
> py manage.py migrate
```

## [Admin and Apps](https://www.youtube.com/watch?v=BJfyATa9nX0&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=3)

```
> py manage.py createsuperuser
Username: <user>
Email address: <email>
Password: <pwd>
```

Install text widget and use for text fields.

```
> pip install django-tinymce4-lite
```

Follow the [Admin and Apps - Django Tutorial](https://pythonprogramming.net/admin-apps-django-tutorial/) text version.

## [Views and Templates](https://www.youtube.com/watch?v=j9elKTmCEhY&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=4)

https://pythonprogramming.net/views-templates-django-tutorial/?completed=/admin-apps-django-tutorial/

## [CSS](https://www.youtube.com/watch?v=a3d_nyccpM8&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=5)

https://pythonprogramming.net/css-django-tutorial/?completed=/views-templates-django-tutorial/

## [User Registration](https://www.youtube.com/watch?v=riXD5lSInJ4&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=6)

https://pythonprogramming.net/user-registration-django-tutorial/?completed=/css-django-tutorial/

## [Messages and Includes](https://www.youtube.com/watch?v=0VGJPg0SQIY&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=7)

https://pythonprogramming.net/messages-django-tutorial/?completed=/user-registration-django-tutorial/

## [User Login and Logout](https://www.youtube.com/watch?v=79A1YoQ5ZJc&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=8)

https://pythonprogramming.net/user-login-logout-django-tutorial/?completed=/messages-django-tutorial/

## [Linking models with Foreign Keys](https://www.youtube.com/watch?v=Rju5qdU0e58&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=9)

https://pythonprogramming.net/foreign-keys-django-tutorial/?completed=/user-login-logout-django-tutorial/

# lab-py-django

Experimenting with Python and [Django](https://www.djangoproject.com/) for web development. Checking tutorial series - [Django Web Development with Python](https://www.youtube.com/watch?v=yD0_1DPmfKM&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3)

## [Introduction](https://www.youtube.com/watch?v=yD0_1DPmfKM&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3)

```
> pip install django  #In video the 2.1.x is used. But I have installed the 3.0.4
```

Django considers a website to be a collection of apps. (i.e. store app, blog app). Official Django tutorial is [here](https://docs.djangoproject.com/en/3.0/intro/tutorial01/).

If interested, you can read about Flask vs Django topics.

```
> django-admin startproject crawlers  #The crawlers is going to be as a core.
```

```
> py manage.py startapp crawlers_auto  #The main is going to be as an app within.
```

```
> py manage.py runserver  #run the site by default on http://127.0.0.1:8000/.
```

## [Models](https://www.youtube.com/watch?v=aXxIjeGR6po&list=PLQVvvaa0QuDe9nqlirjacLkBYdgc2inh3&index=2)

Create/define model -> make migrations -> migrate model. `(model == table)`

If making/updating the model you have to do migrations. But before running the migrations, we have to actually install the `crawlers_auto` app. The initial create operation was not enough. Apparently you have to also do the `install`. Add sub-app into config of core app.

```
> py manage.py makemigrations
> py manage.py migrate
```

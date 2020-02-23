# Django Core Fundamentals

This guide will cover the core fundamentals of the Django framework. This is meant to be used as a reference. There is no specific project associated with this guide and can be used along with any project.

## Prerequisite

* You are familiar with Python
* You understand virtual environments

## What is Django

Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of Web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source.

### Some benefits of Django are

* Ridiculously Fast
  * Django was designed to help developers take applications from concept to completion as quickly as possible.
* Reliable Security
  * Django takes security seriously and helps developers avoid many common security mistakes.
* Exceedingly Scalable.
  * Some of the busiest sites on the Web leverage Django’s ability to quickly and flexibly scale.

[read more here](https://www.djangoproject.com/start/overview/)
___

## Install Django

* *Note: It is best to build apps in a virtual environment*

Django is installed using ```pip```. To install Django run the following command using ```pip``` or ```pip3```.


```pip install django```

This will install the following packages:

```
asgiref==3.2.3
Django==3.0.3
pytz==2019.3
sqlparse==0.3.0
```

* *Note: It is best to build apps in a virtual environment*

Python is now setup to use the Django framework.

___

## Start A Django Project

All Django projects begin with a project. The project is the root folder for everything associated with the project including apps. Django will create this folder with the name specified in the ```django-admin``` command. 

In the code example below. The project is called 'BlogSite'

```django-admin startproject BlogSite```

This will create the following project in the file system as the root directory.
```
BlogSite/
┣ BlogSite/
┃ ┣ __init__.py
┃ ┣ asgi.py
┃ ┣ settings.py
┃ ┣ urls.py
┃ ┗ wsgi.py
┗ manage.py
```

**Make sure you navigate into this directory**

Think of this directory as the server. You can run this server but there is no content associated with it. However, this is now a fully functional web server that can be started from the ```manage.py``` file.

### The ```manage.py``` File

The ```manage.py``` file is  command-line utility that lets you interact with this Django project in various ways.


## Start The Server

___

To start the server, run the following command. Since there is no app/website associated with this project yet, it will generated a generic Django landing page.

* *Note: Make sure you are in the directory of the file you are running*

```python manage.py runserver```

Once the server is started, the following information will be shown in the command line. Navigate to the local URL to see Django running.

```Django version 3.0.3, using settings 'BlogSite.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```

*There will be some other output on the command line in regards to warning and migrations. This can be ignored and will be corrected at a later time.*

___

## 
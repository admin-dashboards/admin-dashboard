---
title: "Flask Dashboard GradientAble"
slug: flask-dashboard-gradientable
date: 2020-07-07
language: en
cover: ./flask-dashboard-gradientable.jpg
tags:
 - flask-dashboard
 - gradientable
 - open-source
description: "Gradient Able design coded in Flask."
---

Hello Coders,

This article presents a new [Flask](https://www.palletsprojects.com/p/flask/) admin dashboard generated by the [AppSeed](https://appseed.us) platform on top of [Gradient Able Dashboard](https://codedthemes.com/item/gradient-able-bootstrap-lite/?ref=appseed) design crafted by [CodedThemes](https://codedthemes.com/?ref=appseed).

## Flask Dashboard Features

The starter is released with a basic set of features on Github, under the MIT license. Based on the permissive license, the project can be used for unlimited hobby and commercial projects - App features:

- UI Kit: GradientAble (Free version) provided by CodedThemes
- Codebase: [Flask Dashboard Boilerplate](https://github.com/app-generator/boilerplate-code-flask-dashboard) v1.0.1
- Authentication (via flask_login), Forms validation
- SQLite / PostgreSQL database, SqlAlchemy ORM, Alembic (db migrations)
- Deployment scripts: Docker, Gunicorn, Heroku

> Dashboard Links

- **[Flask Dashboard GradientAble](https://appseed.us/admin-dashboards/flask-dashboard-gradientable)** - the product page
- [Flask Dashboard GradientAble Demo](https://flask-dashboard-gradientable.appseed.us/) - can be tested using default credentials
- [Flask Dashboard GradientAble Sources](https://github.com/app-generator/flask-dashboard-gradientable) - published on Github
- More **[Flask Admin Dashboards](https://appseed.us/admin-dashboards/flask)** - free & paid
- **[Admin Dashboards](https://appseed.us/admin-dashboards)** - Index provided by AppSeed

![Flask Dashboard GradientAble - Open-Source admin dashboard coded in Flask.](https://raw.githubusercontent.com/app-generator/flask-dashboard-gradientable/master/media/flask-dashboard-gradientable-screen.png)

## [Flask](https://www.palletsprojects.com/p/flask/) Framework

[Flask](https://www.palletsprojects.com/p/flask/) is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. Classified as a microframework, Flask is written in Python and it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions.

> Flask Links

- [Flask](https://www.palletsprojects.com/p/flask/) - the official website
- [Flask Documentation](https://flask.palletsprojects.com/)
- [What is Flask](https://docs.appseed.us/what-is/flask) - a comprehensive resource about Flask

<br />

## [GradientAble Dashboard](https://codedthemes.com/item/gradient-able-bootstrap-lite/?ref=appseed)

Gradient Able Free Bootstrap 4 Free/Lite Admin Template is a complete solution for your dashboard creation. The default layout version comes with limited options like Google optimized, font integration, high speed, mature & sophisticated, and extremely well-organized code which makes free Gradient Able a fully flexible solution for any backend application project.

## Set up for development

In case you like the design and decide to build the starter, Python3 should be properly installed in the workstation.  If you are not sure if Python is properly installed, please open a terminal and type `python --version`. The full-list with dependencies and tools required to build the app:

- [Python3](https://www.python.org/) - the programming language used to code the app
- [GIT](https://git-scm.com/) - used to clone the source code from the Github repository
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment.

> Check Python version (using the terminal)

```bash
$ # Check Python version
$ python --version
Python 3.7.2 # <--- All good
```

> Check GIT command tool (using the terminal)

```bash
$ # Check git
$ git --version
$ git version 2.10.1.windows.1 # <--- All good
```

## Codebase structure

The project is coded using blueprints, app factory pattern, dual configuration profile (development and production) and an intuitive structure presented bellow:

> Simplified version

```bash
< PROJECT ROOT >
   |
   |-- app/                      # Implements app logic
   |    |-- base/                # Base Blueprint - handles the authentication
   |    |-- home/                # Home Blueprint - serve UI Kit pages
   |    |
   |   __init__.py               # Initialize the app
   |
   |-- requirements.txt          # Development modules - SQLite storage
   |-- requirements-mysql.txt    # Production modules  - Mysql DMBS
   |-- requirements-pqsql.txt    # Production modules  - PostgreSql DMBS
   |
   |-- .env                      # Inject Configuration via Environment
   |-- config.py                 # Set up the app
   |-- run.py                    # Start the app - WSGI gateway
   |
   |-- ************************************************************************
```

> The bootstrap flow

- run.py loads the .env file
- Initialize the app using the specified profile: Debug or Production
    - If env.DEBUG is set to True the SQLite storage is used
    - If env.DEBUG is set to False the specified DB driver is used (MySql, PostgreSQL)
- Call the app factory method create_app defined in app/init.py
- Redirect the guest users to Login page
- Unlock the pages served by home blueprint for authenticated users

## Build the app

To see the app running locally, we need to clone or download the sources from [Flask GradientAble repository](https://github.com/app-generator/flask-dashboard-gradientable) and follow the instructions provided in the [README](https://github.com/app-generator/flask-dashboard-gradientable/blob/master/README.md) file.

```bash
$ # Get the code
$ git clone https://github.com/app-generator/flask-dashboard-gradientable.git
$ cd flask-dashboard-gradientable
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Install modules - SQLite Database
$ pip3 install -r requirements.txt
$
$ # OR with PostgreSQL connector
$ # pip install -r requirements-pgsql.txt
$
$ # Set the FLASK_APP environment variable (Unix/Mac)
$ export FLASK_APP=run.py
$
$ # Start the application (development mode)
$ flask run
$
$ # Access the dashboard in browser: http://127.0.0.1:5000/
```

Note: To use the app, please access the registration page and create a new user. After authentication, the app will unlock the private pages.

If all goes well, we should see the app running in the browser. 

> Flask GradientAble - Charts Page

![Flask Dashboard GradientAble - Open-Source admin dashboard, the Charts page.](https://raw.githubusercontent.com/app-generator/flask-dashboard-gradientable/master/media/flask-dashboard-gradientable-screen-1.png)

> Flask GradientAble - Google Maps Page

![Flask Dashboard GradientAble - Open-Source admin dashboard, Google Maps Page.](https://raw.githubusercontent.com/app-generator/flask-dashboard-gradientable/master/media/flask-dashboard-gradientable-screen-2.png)

> Flask GradientAble - UI Tables

![Flask Dashboard GradientAble - Open-Source admin dashboard, UI Tables Page.](https://raw.githubusercontent.com/app-generator/flask-dashboard-gradientable/master/media/flask-dashboard-gradientable-screen-3.png)

### Links & Resources

For support please use Github Issues tracker of join the AppSeed community on **Discord**

- [Admin Dashboards](https://appseed.us/admin-dashboards) - Index provided by AppSeed
- [AppSeed Discord](https://discord.gg/fZC6hup) - for 24/7 LIVE Assistance
- [Admin Dashboards](https://github.com/app-generator/admin-dashboards) - a huge index with coded admin dashboards, published on Github
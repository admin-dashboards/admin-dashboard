---
title: "Flask Dashboard Adminator"
slug: flask-dashboard-adminator
date: 2020-02-22
language: en
cover: ./flask-dashboard-adminator-cover.jpg
tags:
 - flask-dashboard
 - admin-dashboards
 - adminator
description: "Adminator, the popular Bootstrap4 Admin template provided by ColorLib is now available as a coded web app in Flask Framework (MIT License)"
---

**Adminator**, the popular Bootstrap4 Admin template provided by ColorLib is now available as a coded web app in [Flask Framework](https://palletsprojects.com/p/flask/) (MIT License) - provided by [AppSeed](https://appseed.us).

## [Adminator Dashboard](https://appseed.us/admin-dashboards/flask-dashboard-adminator)

**Adminator** is a responsive Bootstrap 4 Admin Template. It provides you with a collection of ready to use code snippets and utilities, custom pages, a collection of applications and some useful widgets. This UI kit comes with a clean and modern design that might help you to start faster a new project.  It’s easily customizable and provides you a collection of custom pages, applications, necessary widgets to code a beautiful admin dashboard in less time.

![Flask Dashboard Adminator - Open-Source Flask Dashboard.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-adminator-screen.png)

## Dashboard Links

- [Adminator Flask](https://flask-dashboard-adminator.appseed.us/login.html) - LIVE Demo
- [Adminator Flask](https://appseed.us/admin-dashboards/flask-dashboard-adminator) - Product page, hosted by [AppSeed](https://appseed.us)
- [Adminator Flask](https://docs.appseed.us/admin-dashboards/flask-dashboard-adminator/) - Documentation

## What is [Flask](https://palletsprojects.com/p/flask/)

[Flask](https://palletsprojects.com/p/flask/) is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around Werkzeug and Jinja and has become one of the most popular Python web application frameworks.

Flask is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions.

Starting with Flask is super easy. We need to have Python installed and a few minutes to spare:

```bash
$ pip install flask
```

Create a new file `hello.py` to bootstrap a simple Flask web app.

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
    return 'Hello from Flask'
```

Now, we can execute our Flask app, directly from the terminal:

```bash
$ env FLASK_APP=hello.py flask run
 * Serving Flask app "hello"
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

For more information about **Flask**, please access the [offcial website](https://palletsprojects.com/p/flask/) or the [documentation](https://palletsprojects.com/p/flask/).

## Prepare the environment

To build this free admin dashboard, Python3 should be installed properly in our workstation. If you are not sure if Python is properly installed, please open a terminal and type `python --version`. The full-list with dependencies and tools required to build the app:

- [Python3](https://www.python.org/) - the programming language used to code the app
- [Git](https://git-scm.com/) - used to clone the source code from the Github repository
- A [Github](https://github.com/) account - the invitation to the source code, will be sent on your account.
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment.

> How to check if Python installed

```bash
$ python --version
Python 3.7.2 # <--- All good
```

> Check GIT command tool

```bash
$ # Check git
$ git --version
$ git version 2.10 # <--- All good
```

## Source Code Structure

The boilerplate code is built with a modular structure and the most important files and directories are shown below:

<br />

```bash
< PROJECT ROOT >                          # application root folder
    |
    |--- app/__init__.py                  # application constructor  
    |--- app//assets                      # Img, CSS, Javascript files
    |--- app/templates                    # Jinja2 files
    |            |---<includes>           # Page chunks, components
    |            |---<layouts>            # Layouts
    |            |---<pages>              # Pages
    |                |---- index.html     # Main dashboard page
    |                |---- login.html     # Login page
    |                |---- register.html  # Registration Page
    |                |---- tables.html    # UI Tables
    |                |---- charts.html    # Charts
    |
    |--- requirements.txt                 # Modules and dependencies
    |
    |--- run.py                           # bootstrap the app
    |
    |-----------------------------
```

To build the app and see something on the screen, the build instructions provided in the README file (published on Github) should be enoght. In case you need more information, please access the [product page](https://appseed.us/admin-dashboards/flask-dashboard-adminator) - hosted by AppSeed platform.

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/flask-dashboard-adminator.git
$ cd flask-dashboard-adminator
$
$ # Virtualenv modules installation
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # Install requirements
$ pip3 install -r requirements.txt
$
$ # Set the FLASK_APP environment variable
$ export FLASK_APP=run.py
$
$ # Run the application
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the app in browser: http://127.0.0.1:5000/
```

By visiting the app in browser, we should see the [login page](https://flask-dashboard-adminator.appseed.us/login.html) because guests (unauthenticated) users are redirected to the login page. By default, the app is not provisioned with a default user and we need to create one using the [registration](https://flask-dashboard-adminator.appseed.us/register.html) page.

![Adminator coded in Flask - Login Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-adminator-screen-login.png)

After we pass the authentication, the web app will unlock all private pages and menus:

> Adminator - Calendar Page

![Adminator coded in Flask - Calendar Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-adminator-screen-1.png)

> Adminator - Available Charts

![Adminator coded in Flask - Charts Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-adminator-screen-2.png)

> Adminator - Google Maps Page

![Adminator coded in Flask - Maps Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-adminator-screen-3.png)

### Where to go from here

Grab the source code from the **[official repository](https://github.com/app-generator/flask-dashboard-adminator)**, acces the **[product page](https://appseed.us/admin-dashboards/flask-dashboard-adminator)** or connect with the AppSeed community on [Discord](https://discord.gg/fZC6hup).
Also, might be a good idea to start coding your next admin dashboard using the existing boilerplate code provided by AppSeed:

- [Open-Source Admin Panels](https://appseed.us/admin-dashboards/open-source) - a huge list with free admin panels (MIT License)
- Access the index with [open-source admin panels](https://github.com/app-generator/admin-dashboards) published on Github
- Publish your work here on Admin-Dashboards.com - read [how it works](/how-it-works)

> Thank you for reading!

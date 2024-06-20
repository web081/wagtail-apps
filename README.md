<h1 align="center">
    This project was a demonstration of Git Action CI/CD with Docker, Deployed into AWS 
</h1>
<h1 align="center">
    <picture>
        <source media="(prefers-color-scheme: light)" srcset=".github/wagtail.svg">
        <source media="(prefers-color-scheme: dark)" srcset=".github/wagtail-inverse.svg">
        <img width="343" src=".github/wagtail.svg" alt="Wagtail">
    </picture>
</h1>


Wagtail is an open-source content management system built on Django, with a strong community and commercial support. It's focused on user experience and offers precise control for designers and developers.

![Wagtail screenshot](https://cdn.jsdelivr.net/gh/wagtail/wagtail@main/.github/wagtail-screenshot-with-browser.png)

### Join the Community at Wagtail Space! 🚀

Wagtail Space is coming in June 2024! Don't miss your chance to meet other Wagtailers in person. The Call for Participation and registration for both Wagtail Space 2024 events is open. We'd love to have you give a talk, contribute to a sprint, or join us as an attendee in June.

* [Wagtail Space NL](https://nl.wagtail.space/), Arnhem, The Netherlands. 2024-06-12 - 2024-06-14
* [Wagtail Space US](https://us.wagtail.space/), Philadelphia, PA. 2024-06-20 to 2024-06-22

### 🔥 Features

-   A fast, attractive interface for authors
-   Complete control over front-end design and structure
-   Scales to millions of pages and thousands of editors
-   Fast out of the box, cache-friendly when you need it
-   Content API for 'headless' sites with decoupled front-end
-   Runs on a Raspberry Pi or a multi-datacenter cloud platform
-   StreamField encourages flexible content without compromising structure
-   Powerful, integrated search, using Elasticsearch or PostgreSQL
-   Excellent support for images and embedded content
-   Multi-site and multi-language ready
-   Embraces and extends Django

Find out more at [wagtail.org](https://wagtail.org/).

### 👉 Getting started

Wagtail works with [Python 3](https://www.python.org/downloads/), on any platform.

To get started with using Wagtail, run the following in a [virtual environment](https://docs.python.org/3/tutorial/venv.html):

![Installing Wagtail](.github/install-animation.gif)

```sh
pip install wagtail
wagtail start mysite
cd mysite
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

For detailed installation and setup docs, see [the getting started tutorial](https://docs.wagtail.org/en/stable/getting_started/tutorial.html).

### 👨‍👩‍👧‍👦 GIT ACTION FOR CI/CD AUTOMATION WITH DOCKER
```sh
name: CI/CD Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - name: Checkout code
      uses: actions/checkout@v2

    - name: Set up Docker Buildx
      uses: docker/setup-buildx-action@v1

    - name: Login to DockerHub
      uses: docker/login-action@v1
 check workflow for more details
```



### 📖 Documentation

[docs.wagtail.org](https://docs.wagtail.org/) is the full reference for Wagtail, and includes guides for developers, designers and editors, alongside release notes and our roadmap.

For those who are **new to Wagtail**, the [Zen of Wagtail](https://docs.wagtail.org/en/stable/getting_started/the_zen_of_wagtail.html) will help you understand what Wagtail is, and what Wagtail is _not_.

**For developers** who are ready to jump in to their first Wagtail website the [Getting Started Tutorial](https://docs.wagtail.org/en/stable/getting_started/tutorial.html) will guide you through creating and editing your first page.

**Do you have an existing Django project?** The [Wagtail Integration documentation](https://docs.wagtail.org/en/stable/getting_started/integrating_into_django.html) is the best place to start.

### 📌 Compatibility

_(If you are reading this on GitHub, the details here may not be indicative of the current released version - please see [Compatible Django / Python versions](https://docs.wagtail.org/en/stable/releases/upgrading.html#compatible-django-python-versions) in the Wagtail documentation.)_

Wagtail supports:

-   Django 4.2.x and 5.0.x
-   Python 3.8, 3.9, 3.10, 3.11 and 3.12
-   PostgreSQL, MySQL and SQLite (with JSON1) as database backends

[Previous versions of Wagtail](https://docs.wagtail.org/en/stable/releases/upgrading.html#compatible-django-python-versions) additionally supported Python 2.7, 3.7 and earlier Django versions.

---



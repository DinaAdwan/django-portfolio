# Django Personal Portfolio

A personal portfolio site with a projects showcase and a blog, built with Django during the Gaza Sky Geeks backend programme.

## Features
- **Projects app:** list of projects with title, description, technology and image, plus a detail page for each
- **Blog app:** posts with categories (many-to-many), a page per category, and comments on each post
- Shared base template across apps
- `/` redirects to `/projects/`

## Tech
Python · Django 4.1 · SQLite · Django templates

## Run locally
```bash
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```
Add projects and posts from `/admin/`.

The secret key is read from the `DJANGO_SECRET_KEY` environment variable; a development fallback is used if it isn't set.

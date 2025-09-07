# ALX Travel App

Initial Django project setup with:

- Django REST Framework
- CORS Headers
- Celery (RabbitMQ broker)
- Swagger (drf-yasg) at `/swagger/`
- MySQL configuration via environment variables using `django-environ`.

## Environment Variables

Copy `.env.example` to `.env` and adjust values.

## Basic Commands

Run migrations:
```
python manage.py migrate
```

Create superuser:
```
python manage.py createsuperuser
```

Run server:
```
python manage.py runserver
```

Run Celery worker:
```
celery -A alx_travel_app worker -l info
```

Swagger docs at: http://localhost:8000/swagger/
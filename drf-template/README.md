# DRF Template

This repository is a starter template for building Django REST Framework services.

Use it as a base project, then replace API modules, domain models, and business logic for your own product.

## Why this exists

- Fast project bootstrap with common backend defaults
- Environment-based configuration with django-environ
- PostgreSQL-ready database config out of the box
- CORS support for frontend integration
- OpenAPI + Swagger docs preconfigured

## Included template defaults

- Django 6 + DRF
- Database from DATABASE_URL (PostgreSQL fallback configured)
- DEBUG from environment variables
- CORS configuration from environment variables
- Swagger UI: /api/docs/
- ReDoc: /api/redoc/
- OpenAPI schema: /api/schema/
- Static files:
	- Source directory: static/
	- Collected directory: staticfiles/

## Quick start

1. Create and activate your virtual environment.
2. Install dependencies.
3. Create a .env file in project root.
4. Run migrations.
5. Start the server.

Example commands:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e .
python manage.py migrate
python manage.py runserver
```

## Environment variables

Create .env in project root:

```env
DEBUG=True
DATABASE_URL=postgresql://postgres:postgres@localhost:5432/postgres

# CORS
CORS_ALLOW_ALL_ORIGINS=True
# CORS_ALLOWED_ORIGINS=http://localhost:3000,http://127.0.0.1:3000
```

Notes:

- Use CORS_ALLOW_ALL_ORIGINS only for local development.
- In production, set CORS_ALLOW_ALL_ORIGINS=False and define CORS_ALLOWED_ORIGINS.

## How to use this template for a new project

1. Rename the project and app modules to your service name.
2. Set production-safe .env values.
3. Add your apps, models, serializers, views, and routes.
4. Keep shared baseline settings from this template.

## Template scope

This template intentionally includes infrastructure defaults only.

It does not include:

- Domain models
- Authentication flows
- Business-specific APIs
- CI/CD pipeline definitions

Add those according to your project requirements.

# Kittygram

![Main Kittygram workflow](https://github.com/Rufina007/kittygram_final/actions/workflows/main.yml/badge.svg)

Сервис для публикации фотографий котиков с достижениями.

# Технологии

- Python 3.12
- Django 5.1
- Django REST Framework
- PostgreSQL
- Docker / Docker Compose
- Nginx
- GitHub Actions

# Запуск проекта

1. Клонируй репозиторий:

git clone git@github.com:Rufina007/kittygram_final.git
cd kittygram_final

2. Создай файл `.env` по образцу `.env.example`:

POSTGRES_USER=django_user
POSTGRES_PASSWORD=mysecretpassword
POSTGRES_DB=kittygram
DB_HOST=db
DB_PORT=5432
SECRET_KEY=your_secret_key
DEBUG=False
ALLOWED_HOSTS=localhost,127.0.0.1

3. Запусти контейнеры:

docker-compose up -d

4. Выполни миграции и собери статику:

docker-compose exec backend python manage.py migrate
docker-compose exec backend python manage.py collectstatic

# Автор

Rufina007

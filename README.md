# Kittygram

Сервис для публикации фотографий котов.

## Стек технологий

- Python 3.12, Django 5.1
- PostgreSQL 13
- Docker, Docker Compose
- Nginx, Gunicorn
- React, Node.js 18
- GitHub Actions (CI/CD)

## Локальный запуск

1. Клонировать репозиторий
```bash
git clone https://github.com/Zero4411-op/kittygram_final.git
cd kittygram_final

2. Создать .env файл:
cp .env.example .env

3.Запустить контейнеры:
docker-compose up -d

4.Применить миграции и собрать статику:
docker-compose exec backend python manage.py migrate
docker-compose exec backend python manage.py collectstatic --noinput
Проект доступен по адресу: http://localhost:9000
```

## Примеры запросов к API
GET /api/cats/ — список котов
POST /api/cats/ — добавить кота


### Автор
Zero4411-op
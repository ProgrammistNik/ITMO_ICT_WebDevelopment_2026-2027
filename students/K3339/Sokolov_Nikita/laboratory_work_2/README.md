# Лабораторная работа 2 — Вариант 6: Табло победителей автогонок

Django 4.2 + PostgreSQL.

## Требования

- Python 3.9+
- PostgreSQL 

Создать БД `racing_db`, пользователь `postgres`, пароль `postgres` (или задать свои через переменные окружения `POSTGRES_DB`, `POSTGRES_USER`, `POSTGRES_PASSWORD`, `POSTGRES_HOST`, `POSTGRES_PORT`).

## Запуск

```bash
cd students/K3339/Sokolov_Nikita/laboratory_work_2
python3 -m venv .venv
```

Активация venv:
- macOS / Linux: `source .venv/bin/activate`
- Windows: `.venv\Scripts\activate`

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py seed_data
python manage.py runserver
```

Сайт: http://127.0.0.1:8000/

| Логин | Пароль | Роль |
|-------|--------|------|
| admin | admin123 | администратор |
| racer1 | racer123 | пользователь |

## Функционал

- Регистрация и вход
- Список гонок с поиском и пагинацией
- Регистрация на гонку, правка и удаление своей заявки
- Комментарии (тип, рейтинг 1–10, дата заезда)
- Staff в клиенте: CRUD гонок и результатов
- Таблица участников и результатов
- Django-admin: `/admin/`

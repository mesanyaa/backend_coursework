# Система учета медицинских карт пациентов

## Описание проекта
Веб-приложение для учета медицинских карт пациентов, разработанное с использованием Django и MySQL.

## Технологии
- Backend: Python, Django
- База данных: MySQL

## Установка и запуск

1. Создайте виртуальное окружение:
```bash
python -m venv venv
source venv/bin/activate  # для Linux/Mac
```

2. Установите зависимости:
```bash
pip install -r requirements.txt
```

3. Создайте файл .env в корневой директории проекта и добавьте настройки:
```
DEBUG=True
SECRET_KEY=your-secret-key
DB_NAME=medical_records
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_HOST=localhost
DB_PORT=3306
```

4. Примените миграции:
```bash
python manage.py migrate
```

5. Создайте суперпользователя:
```bash
python manage.py createsuperuser
```

6. Запустите сервер разработки:
```bash
python manage.py runserver
```

## Структура проекта
- `medical_records/` - основной проект Django
- `patients/` - приложение для управления пациентами
- `medical_cards/` - приложение для управления медицинскими картами
- `users/` - приложение для управления пользователями
- `api/` - REST API endpoints

## API Endpoints
- `/api/patients/` - управление пациентами
- `/api/medical-cards/` - управление медицинскими картами
- `/api/users/` - управление пользователями

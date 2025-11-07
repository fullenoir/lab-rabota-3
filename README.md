# UserAPIProject2 — Система складского учёта

Назначение: информационная система для автоматизации складского учёта товаров. Реализована по многослойной архитектуре (DAL → BLL → API) с использованием Python, FastAPI, SQLAlchemy и SQLite.

## Установка и запуск
```bash
git clone https://github.com/yourusername/UserAPIProject2.git
cd UserAPIProject2
python -m venv .venv
.venv\Scripts\activate       # Windows
pip install -r requirements.txt
uvicorn main:app --reload

# Структура проекта 
UserAPIProject2/
│ main.py               # Точка входа
│ requirements.txt       # Зависимости
├─ dal/ (Data Access Layer)
│   ├─ database.py       # Настройка БД
│   └─ models.py         # Таблицы SQLAlchemy
├─ bll/ (Business Logic Layer)
│   └─ services.py       # Логика операций
└─ api/ (Presentation Layer)
    └─ routes.py         # Маршруты FastAPI

# Архитектура проекта
main.py
  ├── api/routes.py       # Интерфейс API
  ├── bll/services.py     # Бизнес-логика
  └── dal/database+models # Работа с БД

# Автор
Разработчик: Захаров Даниил Романович
Год: 2025


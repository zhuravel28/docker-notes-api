# Практична робота 2 (Частина 1): Контейнеризація додатку з Docker

## Варіант 1: REST API для нотаток

## Опис проєкту

У цій роботі було контейнеризовано Node.js/Express REST API для управління нотатками з використанням PostgreSQL.

Проєкт запускається через Docker Compose та містить два сервіси:

- `app` — Node.js/Express REST API
- `db` — база даних PostgreSQL

## Функціональні можливості API

- `GET /notes` — отримати список усіх нотаток
- `POST /notes` — створити нотатку
- `GET /notes/:id` — отримати нотатку за ID
- `PUT /notes/:id` — оновити нотатку
- `DELETE /notes/:id` — видалити нотатку
- `GET /health` — перевірка стану сервісу

## Структура проєкту

```text
docker-notes-api/
├── src/
│   └── server.js
├── Dockerfile
├── docker-compose.yml
├── .dockerignore
├── .env.example
├── package.json
├── README.md
└── ai-session.md
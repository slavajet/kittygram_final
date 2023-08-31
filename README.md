[![Main Kittygram workflow](https://github.com/slavajet/kittygram_final/actions/workflows/main.yml/badge.svg)](https://github.com/slavajet/kittygram_final/actions/workflows/main.yml)

## Проект KittyGram

KittyGram - это веб-приложение для обмена фотографиями и изображениями котиков. Пользователи могут регистрироваться, загружать свои фотографии котиков, просматривать фотографии других пользователей.

### Функциональность

- Регистрация и аутентификация пользователей.
- Загрузка и просмотр фотографий котиков.

## Стек

- Фронтенд: HTML, CSS, JavaScript, React
- Бэкенд: Python, Django
- База данных: PostgreSQL
- Веб-сервер: Nginx
- Контейнеризация: Docker

## Локальное развертывание

1. Установите Docker на вашем компьютере.

2. Склонируйте репозиторий проекта: `git clone https://github.com/slavajet/kittygram_final.git

3. Перейдите в папку проекта: `cd kittygram`

4. Создайте файл `.env` и укажите необходимые переменные окружения, например:
    ```env
    POSTGRES_DB=kittygramdb
    POSTGRES_USER=kittygramuser
    POSTGRES_PASSWORD=kittygrampassword
    DB_HOST=db
    DB_PORT=5432
    MY_SECRET_KEY='your-secret-key-here'
    ALLOWED_HOSTS=your-domain-or-ip-here,localhost,127.0.0.1
    DEBUG=True
    ```
5. Запустите проект с помощью Docker Compose: `docker-compose up -d`

## Развертывание на сервере

1. Установите Docker и Docker Compose на вашем сервере, следуя инструкциям для вашей операционной системы.
2. Склонируйте репозиторий проекта:
    ```
    git clone https://github.com/slavajet/kittygram_final.git
    ```
3. Перейдите в папку проекта:
    ```
    cd kittygram_final
    ```
4. Создайте файл `.env` в корневой папке проекта и укажите необходимые переменные окружения, например:
    ```env
    POSTGRES_DB=kittygramdb
    POSTGRES_USER=kittygramuser
    POSTGRES_PASSWORD=kittygrampassword
    DB_HOST=db
    DB_PORT=5432
    MY_SECRET_KEY='your-secret-key-here'
    ALLOWED_HOSTS=your-domain-or-ip-here,localhost,127.0.0.1
    DEBUG=False
    ```

5. Запустите проект с помощью Docker Compose Production:

    ```bash
    docker-compose.productions up -d
    ```

## Автор

Проект разработан [Slava Jet](https://github.com/slavajet).

Связаться со мной можно по электронной почте: slavacaas@yandex.ru

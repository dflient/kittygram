## Kittygram

Kittygram - социальная сеть для владельев котов, где они делятся фотографиями и достиженями своих питомцев

## Стек 

#Python 3.9 #Django #Docker #REST Framework #Nginx #Pillow #Djoser #Gunicorn #Node.js

# Запуск приложения

Для работы с БД Postgres требуется создать несколько переменных окружения:
POSTGRES_DB=kittygram
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
DB_HOST=db
DB_PORT=5432
SECRET_KEY=...
На сервере необходимо установить утилиту Docker Compose: 
sudo apt update
sudo apt-get install docker-compose-plugin
В директорию проекта копируем файл docker-compose.production.yml и запускаем Docker Compose: sudo docker сompose up

# URL проекта

Добавить питомца: POST /cats/add

Редактировать питомца: PUTCH /cats/edit

Просмотр питомца: GET /cats/{cat_id}

# Автор проекта

Пастунов Даниил
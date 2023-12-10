## Курсовая 6. Основы веб-разработки на Django

### 1. Для запуска приложения необходимо настроить виртуальное окружение и установить все необходимые зависимости с помощью команд:
        1- python -m venv venv
        2- venv\Scripts\activate
        3- pip install -r requirement.txt


### 2. Для запуска celery:
        1- celery -A config worker -l info  

### 3. Для запуска redis:
        1- sudo apt-get update
        2- sudo service redis-server start
        3- redis-cli
        4- ping
        
        Если PONG - подключен


### 4. Для заполнения моделей данными необходимо выполнить следующую команду:
        1- python manage.py add_blog
        2- python manage.py add_mailing


### 5. Для работы с переменными окружениями необходимо заполнить файл
    - .env

### 6. Для создания администратора (createsuperuser)
    - заполните поля email, PASSWORD. users/management/commands/csu.py

    1- python manage.py csu

### 7. Для запуска приложения: 

    - python manage.py runserver

### 8. Для отправки рассылки из командной строки:
    - python manage.py sendmessage N, где N - это PK рассылки (узнать PK рассылки можно в админке)

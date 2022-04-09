FlaskLearning
==

Источник [The Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)

Chapter 1: Hello, World!
--

Подключение модуля venv

```bash
cd microblog
python3 -m venv venv
```

Активация venv для Linux

```bash
source venv/bin/activate
```
Или для Windows

```bash
source venv/Scripts/activate
```

Деактивация venv

```bash
deactivate
```

Установка пакетов

```bash
pip install flask
pip install python-dotenv
```

Chapter 2: Templates

Ничего важного

Chapter 3: Web Forms
--

Установка пакетов

```bash
pip install flask-wtf
```

Chapter 4: Database
--

Установка пакетов

```bash
pip install flask-sqlalchemy
pip install flask-migrate
```

### Создание модели и миграции

Сначала требуется инициализировать миграцию

```bash
flask db init
```

Создаем модель, например User. Выполнить создание миграции

```bash
flask db migrate -m "users table"
```

И применить изменения в БД

```bash
flask db upgrade
```

Для работы с объектами проекта можно использовать команду

```bash
flask shell
```

Chapter 5: User Logins
--

Установка пакетов

```bash
pip install flask-login
pip install email-validator
```

Chapter 6: Profile Page and Avatars
--

Добавляем поля в модель. Создаёт новую миграцию и применяем ее к БД

```bash
flask db migrate -m "new fields in user model"
flask db upgrade
```

Chapter 7: Error Handling
--

Добавляем окружение в .flaskenv

```bash
FLASK_ENV=development
```

Установка модуля SMTP

```bash
python -m smtpd -n -c DebuggingServer localhost:8025
```

Chapter 8: Followers
--

Добавляем поля в модель. Создаёт новую миграцию и применяем ее к БД

```bash
flask db migrate -m "followers"
flask db upgrade
```

Добавлены тесты.

Chapter 9: Pagination
--

Chapter 10: Email Support
--

Chapter 11: Facelift
--

Chapter 12: Dates and Times
--

Chapter 13: I18n and L10n
--

Chapter 14: Ajax
--

Chapter 15: A Better Application Structure
--

Chapter 16: Full-Text Search
--

Chapter 17: Deployment on Linux
--

Chapter 18: Deployment on Heroku
--

Chapter 19: Deployment on Docker Containers
--

Chapter 20: Some JavaScript Magic
--

Chapter 21: User Notifications
--

Chapter 22: Background Jobs
--

Chapter 23: Application Programming Interfaces (APIs)
--


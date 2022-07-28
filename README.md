![example workflow](https://github.com/zlightho/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

# yamdb_final
## API для проекта yatube

Yatube это социальный блог в котором реализован следующий функционал.

- Добавление постов
- Возможность добовлять комментарии к постам
- Возможность подписываться на авторов постов
- Принадлежность постов к группам
- ✨Аутентификация с помощью JWT✨

## Как запустить проект:

Cоздать и активировать виртуальное окружение:
> Для mac/linux
```sh
python3 -m venv env
```
> Для Windows:
```sh
venv\Scripts\acrivate
```
Обновить pip:
```sh
python3 -m pip install --upgrade pip
```
Установить зависимости из файла requirements.txt:
```sh
pip install -r requirements.txt
```
Выполнить миграции:
> Для mac/linux
```sh
python3 manage.py migrate
```
> Для Windows:
```sh
python manage.py migrate
```

Запустить проект:
> для Windows:
```sh
python manage.py runserver
```
> для Linux:
```sh
python3 manage.py runserver
```
Шаблон env-файла.

```sh
DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres
POSTGRES_USER=пользователь
POSTGRES_PASSWORD=пароль
DB_HOST=db
DB_PORT=5432
SECRET_KEY = '' #секретный ключ Django
EMAIL = 'yambd@yambd.com'
```

Как запускать проект?

```sh
cd infra/
docker-compose up
```

Для запуска тестов.
Прописать команду pytest в папке api_yamdb


## Авторы

Михайлов Артем - https://github.com/zlightho
Немков Максим - https://github.com/jamsi-max/
Шайдуллин Руслан - https://github.com/rusiich

## Лицензия

MIT

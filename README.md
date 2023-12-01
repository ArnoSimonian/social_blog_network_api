# API для социальной сети блогеров


### Описание

Проект является полноценным API для [социальной сети блогеров](https://github.com/ArnoSimonian/social_blog_network).


### Установка

1. Клонируйте репозиторий и перейдите в него в командной строке:

```
  git clone https://github.com/ArnoSimonian/social_blog_network_api.git
  cd social_blog_network_api
```

2. Cоздайте и активируйте виртуальное окружение:

```
  python3 -m venv venv
  # Для Linux/macOS:
  source venv/bin/activate
  # Для Windows:
  source venv/Scripts/activate
```

3. Установите зависимости из файла requirements.txt:

```
  python -m pip install --upgrade pip
  pip install -r requirements.txt
```

4. Выполните миграции:

```
  python manage.py migrate
```

5. В папке с файлом manage.py выполните команду, чтобы запустить проект:

```
  python manage.py runserver
```


### Примеры запросов к API

- Получение списка всех публикаций:

GET ```api/v1/posts/```

- Создание публикации:

POST ```api/v1/posts/```

- Обновление публикации:

PUT ```api/v1/posts/{id}/```

- Частичное обновление комментария:

PATCH ```api/v1/posts/{post_id}/comments/{id}/```

- Подписка на автора:

POST ```api/v1/follow/```

- Информация о сообществе:

GET ```api/v1/groups/{id}/```

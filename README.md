# Парсер фильмов с сайта [tmdb](https://www.themoviedb.org/)

Потребуется `API` ключ - [инструкция по получению](https://developers.themoviedb.org/4/auth/create-access-token)

## Как установить

Для запуска скриптов у вас уже должен быть установлен Python 3.

- Скачайте код
- Установите библиотеки командой `pip install -r requirements.txt`

## hello_api_TMDB.py

Используется для проверки `API` ключа. Просит пользователя ввести `API` ключ.

Если ключ подошел:

![Example](https://user-images.githubusercontent.com/58470881/191806793-50108955-a83a-43d3-9cee-ba493259d3b4.png)

Если ключ не подошел:

![Example](https://user-images.githubusercontent.com/58470881/191808398-c8295842-9ee2-4a69-b13b-a733fdf0da49.png)

## make_own_db.py

Создает базу данных из 1000 фильмов и сохраняет ее в папке со скриптом в файл `MyFilmDB.json`

Отображает прогресс в процентах:

![Example](https://user-images.githubusercontent.com/58470881/191808365-59eb0cba-e656-4b9a-acf2-52ab37ca8026.png)


## search_in_db.py

Поиск фильма в базе данных по его названию:

![Example](https://user-images.githubusercontent.com/58470881/191808329-05bb14db-c946-49c2-995b-e6087a62c417.png)

## find_similar.py

Поиск похожих фильмов в локальной базе по введенному названию фильма.

В результате выводит список из 8 фильмов: 

![Example](https://user-images.githubusercontent.com/58470881/191808381-d1c4e440-5f43-4bbe-ae5f-87a7cafb91a5.png)

## own_db_helpers.py

Получает на вход путь к файлу с базой данных о фильмах. Если путь верный, то возвращает данные из файла в виде словаря.

## tmdb_helpers.py

Содержит вспомогательные функций для работы с `tmdb API`.

# Финальная аттестация SkyPro

## Вариант №1. Тестирование сервиса полезных продуктов Алтайвита.

### Задачи проекта:

- Составьте в excel чек-лист наиболее важных на ваш взгляд проверок для функционала поиска на платформе.
- Составить коллекцию Postman, которая поможет провести смоук-тест корзины и инструкцию по работе с ней.
- Составить SQL запросы по имеющейся информации о таблицах и их связях.
- Написать не менее двух API и двух UI тестов на функционал корзины интернет-магазина.
- Представить проверяющему работу, выполненную на шагах 1-4, показать выполнение запросов и интерфейс приложения.

### Полезные ссылки:
- [Ссылка на требования](https://www.notion.so/1-b26e4c69b2894418a5f12b6bc2a4dd91)
- [Ссылка на тестируемый сервис Алтайвита](https://altaivita.ru/)

#### Проект содержит папки:

- **pages** - в данной папке находятся файлы с методами страниц сервиса Кинопоиск.

- **test** - в данной папке находятся файлы с UI и API тестами.

- **api** - в данной папке находятся файлы с методами API Кинопоиска.

#### Проект содержит файлы:

- **requirements.txt** - файл с используемыми зависимостями в проекте. Установить зависимости на тестовый стенд можно командой **pip install -r requirements.txt**

- **conftest.py** - файлы с фикстурами, используемыми в проекте.

- **config.json** - файл с данными, которые используются для авторизации на сайте (логин и пароль), url адреса для ui и api тестов, содержит также информацию о заголовке и токене, передаваемых в api тестах.

- **AuthPageKinopoisk.py** - содержит методы класса страницы авторизации на сайте.

- **MainPageKinopoisk.py** - содержит методы класса главной страницы сайта, страницы результатов поиска. В данном файле находятся методы: обработка капчи, ввод запроса в модуль поиска, сбор информации по подсказкам к поиску, нажатие нопки поиска, получения информация на странице результата поиска, методы поиска фильма или сериала, персоны и ошибочного (пустого поиска).

- **FilmSeriesPageKinopoisk.py** - файл с методами класса персональной страницы фильма, сериала или персоны. Здесь находятся методы поиска элемента на странице и нажатия на него, нахождение элемента и считывание его текста (и дальнейший его возврат), нахождение кнопок, контроль установленной оценки, установка, изменение и удаление оценки.

- **UserPageKinopoisk.py** - файл с методами класса страницы пользователя. Здесь находятся методы: переход в личный кабинет пользователя, метод позволяющий открыть необходимый раздел в кабинете, метод собирающий информацию в разделе Фильмы и метод для раздела Оценки.

- **FilmTvSeriesApi.py** - содержит методы класса поиска фильма или сериала с использованием Api. Методы поиска фильма/сериала по названию, id, дополнительным полям.

- **PersonAPi.py** - содержит методы класса поиска персоны с использованием Api. Методы поиска персоны по имени и фамилии, id.

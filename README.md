# Проект Tree Menu
Доступ к admin-панели: username: admin, password: admin
## Описание
Проект тестового задания для Junior Python Backend Developer вакансии от UpTrader, 
реализовывающий древовидное меню согласно условиям ТЗ. \
Список условий:
1) Меню реализовано через template tag
2) Все, что над выделенным пунктом - развернуто. Первый уровень вложенности под выделенным пунктом тоже развернут.
3) Хранится в БД.
4) Редактируется в стандартной админке Django
5) Активный пункт меню определяется исходя из URL текущей страницы
6) Меню на одной странице может быть несколько. Они определяются по названию.
7) При клике на меню происходит переход по заданному в нем URL. URL может быть задан как явным образом, так и через named url.
8) На отрисовку каждого меню требуется ровно 1 запрос к БД
## Запуск проекта
Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/doomkirov/tree_menu.git
```
```
cd tree_menu
```
Установить виртуальное окружение и активировать его
>Windows:
> ```python -m venv venv```
>Linux:
> ```python3 -m venv venv```

>Windows:
> ```venv source/scripts/activate```
>Linux:
> ```source venv/bin/activate```

Установить зависимости из файла requirements.txt
```
pip install -r requirements.txt
```
База данных проекта уже наполнена и доступна в каталоге, однако если это не так, необходимо создать суперпользователя для доступа к административной панели
>Windows:
> ```python manage.py createsuperuser```
>Linux:
> ```python3 manage.py createsuperuser```

Проект готов к запуску!
>Windows:
> ```python manage.py runserver```
>Linux:
> ```python3 manage.py runserver```

Чтобы открыть начальную страницу проекта, перейдите по ссылке - http://127.0.0.1:8000/ \
Чтобы открыть административную панель, перейдите по ссылке - http://127.0.0.1:8000/admin \
Имя пользователя: admin, Пароль: admin
## Использованные технологии
Django 4.2.7,
Python 3.12
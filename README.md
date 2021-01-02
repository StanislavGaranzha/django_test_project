<<<<<<< HEAD
# django-simbirsoft
## Тестовый проект для практикума

Приложение для создания простых текстовых заметок.

Общий для всех пользователей функционал &ndash; доступ к главной странице.

Функционал для анонимных пользователей :
1. Зарегистрироваться &ndash; `/users/signup/`
2. Авторизоваться &ndash; `/users/login/`

Функционал для зарегистрированных пользователей:
1. Создать новую заметку &ndash; `/note/new/`
2. Просмотреть список всех своих заметок &ndash; `/author/{author_id}/`
3. Редактировать свою заметку &ndash; `/note/{note_id}/edit/`
4. Удалить свою заметку &ndash; `/note/{note_id}/delete/`
5. Выйти из текущего сеанса &ndash; `/users/logout/`

Пермишены:
1. Анонимным пользователям не доступно ничего из функционала для зарегистрированных пользователей, при попытке доступа &ndash; редирект на страницу входа (login).
2. Зарегистрированным пользователям не доступен CRUD для не своих заметок, прп попытке доступа выводится кастомизированная 403-страница.

***
#### Инструкция по деплою приложения на вашей машине

1. Убедитесь, что запущен Docker.
2. Клонируйте в любое удобное место этот репозиторий:

`git clone https://github.com/StanislavGaranzha/django-simbirsoft`

3. Перейдите через CLI в папку с клонированным репозиторием и выполните следующие команды:
- `docker-compose up -d --build` &ndash; собрать приложение и сделать его первоначальный запуск
- `docker-compose down` &ndash; остановить работу приложения
- `docker-compose run web python manage.py migrate` &ndash; сделать необходимые миграции
- `docker-compose up` &ndash; окончательно запустить приложение.
=======
# django_test_project
## Тестовый проект для практикума

Приложение для создания простых текстовых заметок.

Общий для всех пользователей функционал &ndash; доступ к главной странице.

Функционал для анонимных пользователей :
1. Зарегистрироваться &ndash; `/users/signup/`
2. Авторизоваться &ndash; `/users/login/`

Функционал для зарегистрированных пользователей:
1. Создать новую заметку &ndash; `/note/new/`
2. Просмотреть список всех своих заметок &ndash; `/author/{author_id}/`
3. Редактировать свою заметку &ndash; `/note/{note_id}/edit/`
4. Удалить свою заметку &ndash; `/note/{note_id}/delete/`
5. Выйти из текущего сеанса &ndash; `/users/logout/`

Пермишены:
1. Анонимным пользователям не доступно ничего из функционала для зарегистрированных пользователей, при попытке доступа &ndash; редирект на страницу входа (login).
2. Зарегистрированным пользователям не доступен CRUD для не своих заметок, при попытке доступа выводится кастомизированная 403-страница.

***
#### Инструкция по деплою приложения на вашей машине

1. Убедитесь, что запущен Docker.
2. Клонируйте в любое удобное место этот репозиторий:

`git clone https://github.com/StanislavGaranzha/django_test_project`

3. Перейдите через CLI в папку с клонированным репозиторием и выполните следующие команды:
- `docker-compose up -d --build` &ndash; собрать приложение и сделать его первоначальный запуск
- `docker-compose down` &ndash; остановить работу приложения
- `docker-compose run web python manage.py migrate` &ndash; сделать необходимые миграции
- `docker-compose up` &ndash; окончательно запустить приложение.
>>>>>>> d6dbcf364bc91616fa6f93d1ffef67d09123acc7

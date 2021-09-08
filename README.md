# Greetings traveller

Мы рады, что вы приступили к выполнению 1 задания из курса middle-python разработчик.
 
Описание структуры и порядок выполнения проекта:
1. `schema_design` - раздел c материалами для новой архитектуры базы данных.
2. `sqlite_to_postgres` - раздел с материалами по миграции данных.
3. `movies_admin` - раздел с материалами для панели администратора.

Успехов!

## Запуск

1. Сначала необходимо запустить контейнер с постгресом и проинициализировать бд
```shell
sudo docker-compose up db
```
2. После успешной инициализации бд необходимо собрать контейнер со скриптом выгрузки данных
и запустить этот скрипт
```shell
sudo docker-compose up --build etl
```
3. Далее необходимо собрать контейнер с приложением на джанго
```shell
sudo docker-compose up --build etl
```
4. В браузере зайти в админку джанго с кредами login: root, pass: 1 http://127.0.0.1:8000/admin


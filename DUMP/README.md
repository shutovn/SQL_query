# RUN training DB - Запуск учебных СУБД.
Для полноценного обучения и закрепления изученного материала необходимы тестовые СУБД.

Из директории DUMP/docker с помощью docker-compose и docker можно запустить одну из двух самых популярных СУБД: MySQL and PostgreSQL или сразу обе.
Для корректного запуска обучающих СУБД, необходимо установленные [docker](https://docs.docker.com/engine/install/) и [docker-compose](https://docs.docker.com/compose/install/). Перед первым запуском необходимо переименовать файл DUMP/docker/example.env в DUMP/docker/.env и отредактировать переменные под свои предпочтения.

# Connection - Подключение.

mysql -uroot -h 127.0.0.1 -P33061 -p

psql -Upostgres -h 127.0.0.1 -p54321

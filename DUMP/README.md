# RUN training DB - Запуск учебных СУБД.
Для полноценного обучения и закрепления изученного материала необходимы тестовые СУБД.

Из директории DUMP/docker с помощью docker-compose и docker можно запустить две одни из самых популярных СУБД: MySQL and PostgreSQL.

# Connection - Подключение.

mysql -uroot -h 127.0.0.1 -P33061 -p

psql -Upostgres -h 127.0.0.1 -p54321

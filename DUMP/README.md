# RUN training DB - Запуск учебных СУБД.
Для полноценного обучения и закрепления изученного материала необходимы тестовые СУБД.

Из директории DUMP/docker с помощью docker-compose и docker можно запустить одну из двух самых популярных СУБД: MySQL and PostgreSQL или сразу обе.
Для корректного запуска обучающих СУБД, необходимо установленные [docker](https://docs.docker.com/engine/install/) и [docker-compose](https://docs.docker.com/compose/install/). Перед первым запуском необходимо переименовать файл DUMP/docker/example.env в DUMP/docker/.env и отредактировать переменные под свои предпочтения.

# Connection - Подключение.

mysql -uroot -h 127.0.0.1 -P33061 -p

psql -Upostgres -h 127.0.0.1 -p54321


# Example Databases
Примеры баз данных. Учебная база от mysql с многообещающим названием World. Так же в данном разделе представлена база с информацией по covid19, не сложная, но со значительно большими данными.

## World [world database](https://dev.mysql.com/doc/index-other.html)
Для ее использования, достаточно взять дамп из проекта и загрузить его в СУБД.
```bash
cd ~/MyGitProjects/SQL/DUMP
mysql -u root -h 127.0.0.1 -P33061 -p < world.sql
```

## COVID-19 Data Hub [covid19datahub](https://covid19datahub.io/index.html)
Цель COVID-19 Data Hub — предоставить исследовательскому сообществу унифицированный набор данных путем сбора детальных данных о случаях заболевания по всему миру, объединенных с экзогенными переменными, которые помогут лучше понять COVID-19.  

Для ее использования, необходимо перейти на страницу [Центр загрузки](https://covid19datahub.io/articles/data.html) и выбрать необходимый набор данных.  

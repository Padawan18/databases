
## Задание 1.
1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.
1.2. Создайте учётную запись sys_temp.

![task 1 ](https://github.com/Padawan18/databases/blob/main/mysql6.png)

1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)

![task 1 ](https://github.com/Padawan18/databases/blob/main/mysql2.png)


1.4. Дайте все права для пользователя sys_temp.

![task 1 ](https://github.com/Padawan18/databases/blob/main/mysql5.png)

1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

![task 1 ](https://github.com/Padawan18/databases/blob/main/mysql1.png)

1.6. Переподключитесь к базе данных от имени sys_temp.

1.6. По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.

1.7. Восстановите дамп в базу данных.

1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)

![task 1 ](https://github.com/Padawan18/databases/blob/main/mysql4.png)



## Задание 2. Kibana
Установите и запустите Kibana.
Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty.

![task 2 ](https://github.com/Padawan18/databases/blob/main/2.1.png)


## Задание 3. Logstash
Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx.

![task 3 ](https://github.com/Padawan18/databases/blob/main/3.png)

## Задание 4. Filebeat.
Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx, которые были отправлены через Filebeat.

![task 4 ](https://github.com/Padawan18/databases/blob/main/4.png)

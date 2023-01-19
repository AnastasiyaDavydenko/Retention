# Retention

## Входные данные

Есть база данных в ClickHouse некоторого приложения "Лента новостей", которая собирает информацию о просмотрах и лайках пользователей.
В базе есть два типа пользователей: те, кто пришел через рекламу (ads), и те, кто пришел через органические каналы (organic).

## Задание

Проанализировать и сравнить Retention пользователей, пришедших через разные каналы (ads и organic).

## Решение
В Superset с помощью SQL запроса была построена метрика Retention в разрезе канала привлечения пользователей
![Retention](https://user-images.githubusercontent.com/122218714/213485493-c0623139-98bd-4020-a316-62c062e0ff17.png)

## Вывод

Retention у organic выше, чем у ads. Retention у organic и ads ведет себя схожим образом: на второй день после начала использования приложения возвращаются около 30 % пользователей, в течение последующих 20 дней происходит отток и остается не более 5% пользователей.

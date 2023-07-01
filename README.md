# ELK Demo
Для выполнения требуется наличие Mac/Linux с установленным Docker.

## Что сделано
1. добавлена конфигурация logstash/clickstream.conf для разбора лога logstash/weblog.csv

## Инструкция
1. Инфраструктура поднимается командой docker compose up -d. Запускаются контейнеры elasticsearch и    kibana
2. Загрузите данные веб-логов, выполнив команду `./load_data.sh`
3. Можно перейти по адресу http://localhost:5601 и создать dashboard, показывающий распределение запросов с разными кодами ответов (status) по времени

## Илюстрация (screenshot dashdoard)

![Dashboard Status/Time](https://github.com/mzabolotnov/pic_storage_repository/raw/main/dashboard_status_kibana.png)

# Практическое задание №1. Сбор логов

Выполнил Мерзликин Максим, группа ББМО-01-23

## `rsyslog`

### Установка `rsyslog` на сервер

![](screenshots/Установка_rsyslog.png)

![](screenshots/active_rsyslog.png)

### Настройка модулей `rsyslog`

![](screenshots/rsyslog_config.png)

### Добавление правил обработки логов

![](screenshots/rsyslog_config_2.png)

### Установка `rsyslog` на клиент

![](screenshots/rsyslog_install_client.png)

![](screenshots/active_rsyslog_client.png)

### Добавление правила пересылки логов на сервер

![](screenshots/rule_client_rsyslog.png)

### Просмотр полученных логов на сервере

![](screenshots/ssh_logs.png)

## Grafana Loki

### Редактирование compose-файла с целью отключения компонента `promtail` на сервере

![](screenshots/loki_grafana_config.png)

### Запуск Loki

![](screenshots/loki_grafana_install.png)

### Редактирование конфигурации `promtail` на клиенте

![](screenshots/comfig_and_docker_yaml.png)

### Просмотр логов клиента в Grafana

![](screenshots/работает.png)

## Signoz

### Запуск Signoz

Установка согласно https://signoz.io/docs/install/docker/#install-signoz-using-docker-compose

![](screenshots/signoz_install.png)

### Рабочая панель Signoz

![](screenshots/signoz_menu.png)

### Редактирование конфигурации клиентского приложения для отправки данных в Signoz

Используемое приложение - https://github.com/SigNoz/sample-nodejs-app/

### Запуск клиентского приложения

![](screenshots/docker_node_js.png)

### Информация о приложении в Signoz

![](screenshots/work_signoz.png)


# Практическая работа №5. Threat Hunting

Выполнил Мерзликин Максим, ББМО-01-23

Для работы были использованы уже ранее созданные в [ПРЗ №3](../prz_3/) стенды Wazuh.

## Установка и настройка IDS Suricata

Установка IDS Suricata:

![](./screenshots/installing_suricata.png)

Загрузка правил обнаружения:

![](./screenshots/install_rules_suricata.png)

Настройка переменных конфигурации в файле `/etc/suricata/suricata.yaml`:

![](./screenshots/suricata_yaml_config.png)

Настройка импорта логов Suricata в Wazuh и перезапуск агента:

![](./screenshots/wazuh_rule_suricata.png)

![](./screenshots/new_rule_wazuh_restart.png)

## Установка и настройка Yara

### Настройка агента

Загрузка и распаковка дистрибутива:

![](./screenshots/Yara_download.png)

Установка Yara:

![](./screenshots/yara_install.png)

![](./screenshots/yara_install_2.png)

![](./screenshots/yara_install_3_and_problem.png)

Загрузка YARA-правил:

![](./screenshots/yara_rules_install.png)

Создание скрипта `yara.sh` для Wazuh и установка корректных привилегий согласно документации:

![](./screenshots/yara_rule_make.png)

Настройка правил мониторинга в файле `/var/ossec/etc/ossec.conf`:

![](./screenshots/wazuh_agent_rule.png)

### Настройка сервера

Настройка правил Wazuh для отслеживания изменений и срабатывания правил YARA:

![](./screenshots/wazuh_server_rule.png)

Настройка декодера результатов сканирования Yara:

![](./screenshots/wazuh_server_rule2.png)

Настройка команд Wazuh, который будут запускать сканирование при обнаружении изменений в отслеживаемой директории:

![](./screenshots/wazuh_commands.png)

## Эмуляция атаки

Для осуществления атак в гипервизоре также была развёрнута виртуальная машина с Kali Linux:

![](./screenshots/kali_for_test.png)

Для проверки работы IDS Suricata было запущено сканирование защищаемого узла сканером веб-уязвимостей `nuclei`:

![](./screenshots/nuclei.png)

События, созданные IDS Suricata, выяглядят в логах следующим образом:

![](./screenshots/suricata_match.png)



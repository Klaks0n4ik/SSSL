# Практическая работа №3. Wazuh

Выполнил Мерзликин Максим, ББМО-01-23

## Подготовка стенда, создание виртуальных машин

![](./screenshots/Подготовка_стенда.png)

## Установка сервера Wazuh

![](./screenshots/Установка_wazuh_server.png)

![](./screenshots/Главное_меню_при_входе.png)

## Установка агента Wazuh

![](./screenshots/Установка_агента_1.png)

![](./screenshots/Установка_агента_2.png)

## Подключенный агент в дашборде

![](./screenshots/Агент_в_панели_управления.png)

## Найденные уязвимости в конфигурации по умолчанию

![](./screenshots/Дефолтные_вулны_в_агенте.png)

## Настройка проверки целостности файлов

![](./screenshots/Изменение_проверки_файлов.png)

![](./screenshots/Перезагрузка_агента_с_правилом.png)

### Изменение конфигурационного файла `/etc/hosts`

![](./screenshots/Изменение_файла_хостс.png)

### Срабатывание правила

![](./screenshots/Алерт_на_изменение_файла.png)

## Настройка проверки уязвимостей

![](./screenshots/Насйтрока_проверки_уязвимостей.png)

## Настройка выявления скрытых процессов

### Установка необходимых пакетов

![](./screenshots/Скачивание_необходимых_пакетов.png)

### Настройка мониторинга процессов в агенте Wazuh

![](./screenshots/Настройка_проверки_процессов.png)

### Сборка и запуск руткита

![](./screenshots/Установка_руткита.png)

### На данном этапе произошла ошибка.
### К сожалению, данный пункт задания выполнить не удалось, так как не удавалось запустить нужное ПО для проверки правила.

## Настройка выявления SQL-инъекций

### Установка веб-сервера Apache

![](./screenshots/Установленный_апач.png)

### Конфигурация мониторинга логов Apache

![](./screenshots/Правило_скули.png)

### Срабатывание правила

![](./screenshots/Результат_скуль_индж.png)

## Проверка выявления атаки Shellshock

![](./screenshots/атака_шелшок.png)

![](./screenshots/результат_атаки_шелшок.png)

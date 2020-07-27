# КОД

Контролируемый обмен данными - это механизм построения многоузловой базы из нескольких информационных баз на платформе "1С:Предприятие" с быстрой репликацией всех изменений или их части с поддержкой ссылочной целостности. Главные отличия от РИБ:

* Конфигурации узлов не обязаны совпадать
* Вместо таблиц регистрации изменений используются отметки времени
* Нет квитирования (КОД полагается на гарантированную доставку изменений)
* Изменения передаются не одним большим сообщением, а множеством маленьких, что удобно для обмена через шины вроде Kafka или RabbitMQ
* Есть встроенный механизм контроля ссылочной целостности
* Используется не XML, а JSON

## Архитектура

### Структура сообщения

### Регулярная отправка

#### Выборка изменений

#### Рассмотрение изменений

#### Деление на потоки

#### Отправка изменений

#### Контроль ссылочной целостности

#### Запись сведений об отправке и рассмотрении

### Отправка исторических данных

### Получение сообщений

## Учет изменений в метаданных

### Добавление новых объектов

### Изменение существующих объектов

## Решение проблем

## Открытые вопросы

### Производительность

### Версионирование

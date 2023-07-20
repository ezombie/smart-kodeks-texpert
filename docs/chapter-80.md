# ДАШБОРДЫ

Основаную и логически значимую часть Grafana составляют дашбоды.

Дашборды есть "папки", в которых "сложены" таблицы и/или графики. 
Таблицы и/или графики, в свою очередь, отражают определенную аналитическую и статистическую информацию.

Управление данными на дашбордах осуществляется с помощью задаваемых временных рамок в соответствующей панели, а также с помощью фильтрации по прочим параметрам (см. [Настройки](chapter-60.md)).

Помимо такого способа управления данными, на графиках предоставлена возможность выбора произвольного временного отрезка. [Как это сделать](chapter-60.md#управление-временем-в-дашбордах)

Переходы между дашбордами осуществляются: 
- через клик по названию дашборда на странице - будет открыта страница с избранными дашбордами, последними открытыми и полным списком всех доступных дашбордов;
- через клик по слову General перед именем дашборда - будет открыта страница со всеми доступными дашбордами.

Дашбородов и таблиц/графиков в них на данный момент (16.07.2023) существует уже немалое количество, а именно:

- [Kodeks server metrics](chapter-81.md)
  - [Время нештатного состояния сервера](chapter-81.md#время-нештатного-состояния-сервера)
  - [Разделы с менее чем 10Gb свободного места](chapter-81.md#разделы-с-менее-чем-10gb-свободного-места)
  - [Статусы on-line проверок](chapter-81.md#статусы-on-line-проверок)

- [Kodeks аналитика](chapter-82.md)
  - [Используемые лицензии](chapter-82.md#используемые-лицензии)
  - [Разница между регом и лицензиями](chapter-82.md#разница-между-используемыми-лицензиями-и-регом)
  - [Количество неудачных поисков за сутки](chapter-82.md#количество-неудачных-поисков-за-сутки)
  - [Среднее число запросов kassist](chapter-82.md#среднее-число-запросов-kassist-за-месяц)
  - [Не пользуются системой в течение 60 дней](chapter-82.md#не-пользуются-системой-в-течение-60-дней)
  - [Запросы к БД](chapter-82.md#запросы-к-бд)
  - [Учитываемые документы](chapter-82.md#учитываемые-документы)
  - [Сохранение документов](chapter-82.md#сохранение-документов)
  - [Doc of Service](chapter-82.md#doc-or-service)
  - [Печать документов](chapter-82.md#печать-документов)
  - [Количество лицензий на инсталляции](chapter-82.md#количество-лицензий-на-инсталляции)

- [Биллинг Онлайн](chapter-83.md)
  - [Биллинг Онлайн](chapter-83.md#биллинг-онлайн-1)
  - [Осталось "Документы"](chapter-83.md#осталось--документы-)
  - [Осталось "Поиск"](chapter-83.md#осталось--поиск-)
  - [Осталось "Печать", "Выгрузка", графики аналитики](chapter-83.md#осталось--печать----выгрузка---графики-аналитики)
    - [Средний процент использования лимита документов по всем клиентам](chapter-83.md#средний-процент-использования-лимита-документов-по-всем-клиентам) 
    - [Средний процент использования лимита документов по всем клиентам менеджера](chapter-83.md#средний-процент-использования-лимита-документов-по-всем-клиентам-менеджера)
    - [Осталось "Печать"](chapter-83.md#осталось--печать----выгрузка---графики-аналитики)
    - [Осталось "Выгрузка"](chapter-83.md#осталось--печать----выгрузка---графики-аналитики)
  - [Ошибки подключения к серверам](chapter-83.md#ошибки-подключения-к-серверам)
    - [Проблемы с получением статистики](chapter-83.md#ошибки-подключения-к-серверам)
    - [Варианты ошибок](chapter-83.md#ошибки-подключения-к-серверам)

- [Данные для пролонгации](chapter-84.md)

- Для менеджеров
  - Параметры клиентов
  - Детектирование, что ничего не нашлось

- Загрузка sysinfo в АСРП
  - Статус "принят"
  - Статус не "ок"
  - Загрузка sysinfo в АСРП

- Карточки пользователей
  - Карточки пользователей
  - Топ-20 самых активных пользователей
  
- Контроль версий ПК

- Ошибки БД

- Подключенные пользователи
  - Пользователи, занимающие лицензии на момент получения sysinfo

- Поисковые запросы

- Статистика в разрезе MS ActiveDirectory
  - Запрошенных документов, покрытых лицензией
  - Запрошенных бесплатных документов
  - Запрошенных документов, покрытых лицензией
  - Распечатанных документов
  - Сохраненных документов
  - Активность пользователей в текущем месяце по доменам

- Текущие аварийные ситуации
  - Аварийные ситуации

[Углубимся подробнее в то как и зачем работает каждый дашборд и каждые его график и/или таблица](chapter-81.md)

[Вернуться к Оглавлению, если стало страшно](Readme.md)
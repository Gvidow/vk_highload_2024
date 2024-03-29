# Проектирование высоконагруженной платформы для управления проектами
Курсовая работа в рамках 3-го семестра программы по Веб-разработке ***Образовательного центра VK x МГТУ им.Н.Э.Баумана*** (ex. "Технопарк") по дисциплине "Проектирование высоконагруженных систем"

***Автор:*** Арзмасцев Артем ([Telegram](https://t.me/Gvidow), [VK](https://vk.com/gvidow))

---

#### Содержание:
1. [Тема, функционал и аудитория](#1)
2. [Расчет нагрузки](#2)
3. [Список используемых источников](#3)
---

## Часть 1. Тема, функционал и аудитория<a name="1"></a>

### Тема курсовой работы: ***"Проектирование платформы для управление проектами"***
В качестве примера выбран один из ведущих в мире сервисов управления проектами/тайм-менеджментом - [Trello](https://trello.com/)

### Ключевой функционал сервиса:
- Регистрация и авторизация пользователей;
- Создание контента с разграничениями прав пользования(доски);
- Возможность менять права доступа;
- Добавление и изменение статусов задач;
- Перемещение задач по доскам;
- Добавление комментариев к задачам


### Целевая аудитория:
По данным ***Similarweb[^1]***, аудитория Trello в мире составляет **83,2 млн человек** в месяц.

#### Соотношение пользователей по миру
По данным ***Similarweb[^1]***, самый большой процент аудитории 17.21% приходится на США
![Аудитория Trello](img/world.svg)
- Соединенные Штаты: 17.21%
- Бразилия: 13.76%
- Великобритания: 4.97%
- Германия: 3.39%
- Франция: 3.17%
- Другие: 57.5%

#### Соотношение пользователей по возрастам
- Преимущественно пользователи в возрасте 20-50 лет. Россия
![Возрастное разделение пользователей Trello](img/ages.svg)
- Женщины - 43.45%
- Мужчины - 56.55%

## Часть 2. Расчет нагрузки <a name="2"></a>:

#### Продуктовые метрики
- MAU: 83.2М
- DAU: 19М
- Среднее время проведенное в сервисе: 00:11:26
- Среднее количество просматриваемых страниц при посещении сервиса: 7.77
##### Интенсивность использования разных функций:
- Создание досок
    * Возьмем значение: 0.08 досок в день
- Создание задач
    * Возьмем значение: 3.2 задач в день
- Оставление комментариев
    * Возьмем значение: 2.8 коментариев к задаче или 3.36 в день
- Просмотр досок с задачами
    * Возьмем значение: 5.7
- Смена статусов задач
    * Возьмем значение: 8

#### Технические метрики
##### Размер хранения
- Объем данных пользователя:
    * Аватар 5 МБ
    * Основная информация 200 байт
    * Дополнительная информация 1600 байт
    * **Итого оценочно:** 5001,8 КБ

### Список используемых источников <a name="3"></a>:
[^1]: [Аналитика Trello с Similarweb](https://www.similarweb.com/website/trello.com/#demographics)

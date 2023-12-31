# Вариант 4

Состав команды:

* Кузичев Дмитрий - Работа с БДУ ФСТЭК, проектирование схемы инфраструктуры
* Напольских Никита - сценарии Mitre ATT&CK, поднятие системы

# Описание проекта

Мы познакомимся с Centrifugo, узнаем кто является создателем и как он работает.

# Шаги установки Centrifugo

Условное место установки системы Centrifugo может различаться в зависимости от требований и предпочтений пользователя.

* Установка операционной системы (Использование VirtualBox).
  
* Установка необходимых зависимостей
  * В зависимости от операционной системы может потребоваться установка определенных пакетов и зависимостей.

* Загружаем Centrifugo
  * Получаем установочные файлы Centrifugo с официального репозитория или сайта разработчиков.
  * Распаковываем архив с файлами Centrifugo на сервере или компьютере.

* Установливаем Centrifugo
  * Следуя инструкциям, предоставленным разработчиками Centrifugo, для установки и настройки системы.

* Запуск Centrifugo
  * После установки и настройки Centrifugo, запускаем систему.

# Структурные элементы системы Centrifugo

1. Сервер Centrifugo: это основной компонент системы, который выполняет все основные функции. Он отвечает за обработку запросов, управление соединениями клиентов, передачу данных и управление комнатами.
2. Клиенты: это приложения или устройства, которые подключаются к серверу Centrifugo для обмена данными в режиме реального времени. Клиенты могут быть разработаны на различных платформах, таких как веб, мобильные устройства.
3. Комнаты: Centrifugo позволяет создавать и управлять комнатами, которые служат для группировки клиентов с общими интересами или для организации сообщений определенного типа. 
4. Протоколы: Centrifugo поддерживает различные протоколы для обмена данными, включая HTTP, WebSockets и SockJS. Клиенты могут использовать эти протоколы для подключения к серверу и передачи данных.
5. Аутентификация и авторизация: Centrifugo поддерживает различные методы аутентификации и авторизации, которые позволяют установить и проверить идентичность и права доступа клиентов. Это помогает обеспечить безопасность и предотвратить несанкционированный доступ к системе.
6. Брокеры сообщений: Centrifugo может использовать различные брокеры сообщений, такие как Redis или NATS, для обмена данными между серверами и клиентами. Брокеры сообщений обеспечивают надежную доставку сообщений и резервное копирование данных.

# Схема взаимодействия компонентов системы в Centrifugo может выглядеть следующим образом
1. Клиентские приложения:
- Веб-браузеры
- Мобильные приложения
- Десктопные приложения
2. Centrifugo сервер:
- API
- Websocket
- Механизм аутентификации и авторизации
- База данных для хранения информации о клиентах и каналах
- Кэш для быстрого доступа к данным и уменьшения нагрузки на базу данных
3. Брокер сообщений:
- Например, Redis или NATS
- Используется для обмена сообщениями между Centrifugo сервером и клиентскими приложениями
- Обеспечивает массовую рассылку сообщений по подписанным каналам
4. База данных:
- Например, PostgreSQL или MySQL
- Используется для хранения информации о пользователях, каналах и истории сообщений
5. Подписчики:
- Клиентские приложения, подписанные на определенные каналы
- Получают сообщения через Centrifugo сервер по websocket
6. API клиенты:
- Клиентские приложения, использующие HTTP протокол для взаимодействия с Centrifugo сервером
- Отправляют запросы на добавление пользователей, каналов, отправку сообщений и т.д.
Протоколы:
- WebSocket - используется для поддержки двухсторонней связи между Centrifugo сервером и клиентскими приложениями
- HTTP - используется для взаимодействия с API клиентами
- Redis или NATS - используются в качестве брокера сообщений для обмена сообщениями между сервером и клиентскими приложениями
- PostgreSQL или MySQL - используются в качестве базы данных для хранения информации о пользователях, каналах и истории сообщений

# Описание условного места установки
Система будет установлена в Государственной библиотеке.
Информация в открытом доступе. Некоторые издания, которые связанные с военной тематикой и могут причинить вред людям в закрытом доступе.




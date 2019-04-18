# Эхо сервер

1. [Чему научит](#чему-научит)
2. [Задача](#задача)
3. [Что использовать](#что-использовать)
4. [Начальные шаги](#начальные-шаги)
5. [Другая информация](#другая-информация)
6. [Связанные туториалы](#связанные-туториалы)
7. [Туториал по virtualenv](#туториал-по-virtualenv)

#### Чему научит

Работа с базовыми HTTP методами

#### Задача

Поднять сервер, который будет отвечать на следующие запросы:

- POST `curl -d "name=Max" -X POST <host>:<port>/greet`. Ответ: `{"text": "Hello, max"}`
- GET `curl <host>:<port>/hello/<name>`. Ответ: разметка, внутри которой `<body>Hello, name</body>`
- GET `curl <host>:<port>/?name=Max&age=30`. Ответ: `{"name": "Max", "age": "30"}`

#### Что использовать

Рекомендуется использовать python фреймворк `Flask`, но можно и любой другой фреймфорк/ЯП

#### Начальные шаги

- Форкнуть репу
- Склонировать репу себе
- Создать виртуальное окружение используя `virtualenv` (или любую другую тулзу)
- Активировать виртульное окружение: `source <имя окружения>/bin/activate`
- Установить туда Flask используя пакетный менеджер `pip`: `pip install flask`
- ???
- PROFIT 

#### Другая информация

**Уровень сложности:** начальный

**Специализация:** backend

**Примерное время выполнения:** 1488 минут

## Связанные туториалы (теги)

- [Curl](https://juniorlab.ru/tutorials/curl)
- [Virtualenv](https://juniorlab.ru/tutorials/virtualenv)
- [Pip](https://juniorlab.ru/tutorials/pip)
- [Git](https://juniorlab.ru/tutorials/git)
- [Python](https://juniorlab.ru/tutorials/python)
- [Flask](https://juniorlab.ru/tutorials/flask)
- [HTTP](https://juniorlab.ru/tutorials/http)

## Туториал по virtualenv

`virtualenv` нужен для того, чтобы не засорять глобальное окружение не нужными зависимостями. Так же может понадобиться иметь несколько окружений с разными версиями библиотек.

1. Установить `pip`: `sudo apt-get install python3-pip`
2. Установить `virtualenv`: `sudo pip3 install virtualenv`
3. Создать виртуальное окружение: `virtualenv -p python<версия python> <имя виртуального окружения>` Например: `virtualenv -p python3.6 venv` - создаст виртуальное окружение с версией питона 3.6 и именем venv
4. Активировать виртуальное окружение (для Linux): `source <имя окружения>/bin/activate`. В примере команда будет следующей: `source venv/bin/activate`

После этого войдите в девственное виртуальное окружение, там можно устанавливать ~~все игры~~ нужные библиотеки


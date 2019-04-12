# Эхо сервер

1. [Чему научит](#чему-научит)
2. [Задача](#задача)
3. [Что использовать](#что-использовать)
4. [Начальные шаги](#начальные-шаги)
5. [Связанные туториалы](#связанные-туториалы)

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

## Связанные туториалы

- [Curl](https://juniorlab.ru/tutorials/curl)
- [Virtualenv](https://juniorlab.ru/tutorials/virtualenv)
- [Pip](https://juniorlab.ru/tutorials/pip)
- [Git](https://juniorlab.ru/tutorials/git)
- [Python](https://juniorlab.ru/tutorials/python)
- [Flask](https://juniorlab.ru/tutorials/flask)
- [HTTP](https://juniorlab.ru/tutorials/http)


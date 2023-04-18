# Тесты на проверку получения заеказа по текеру

```Тест проверяет, что на запрос приходит код ответа 200. Присутствует тело ответа json.```

Для запуска этого пакета тестов должны быть установлены: 
- интерпретатор `Python` и среда разработки `PyCharm`
- среда тестирования `Pytest`, библиотека `requests`
- запущен сервер `url.serverhub.praktikum-services.ru` в локальном режиме 
- после запуска сервера его url должен быть внесён в файл `configuration.py` в следующую строку:
```
URL_SERVICE = 'https://ea1dbb2c-89e6-49eb-ac8c-c4c8e5fa828e.serverhub.praktikum-services.ru/'
```

Следует обратить внимание, что при выполнении каждого теста в этом пакете:
- При отправке запроса на получение передаётся номер `track`
- `track` генерируется каждый раз при прохождении тестов с помощью отдельной функции `def create_new_order`

Запуск всех тестов  в Terminal выполняется командой `pytest order_get_test.py`






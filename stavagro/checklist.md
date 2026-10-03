1. # ОТКРЫТИЕ И ОСМОТР САЙТА
☑ Главная страница открывается без ошибок
☑ Контент отображается (блоки «Сервис», «О нас»)
☑ Текст читаемый
☑ Найдена кнопка «Оставить заявку на сервис»
2.# DEVTOOLS → NETWORK
☑ Открыл DevTools (F12)
☑ Перешёл на вкладку Network
☑ Поставил фильтр Fetch/XHR
☑ Включил Keep log
☑ Нашёл запрос calc.php (POST)
☑ URL: https://stavagro.com/php/calc.php
☑ Метод: POST
☑ Формат: x-www-form-urlencoded
☑ Headers просмотрены (Content-Type, Content-Length)
☑ Payload просмотрен:
☑ technical
☑ service
☑ name
☑ phone
☑ email
☑ Response просмотрен: 1
3.# POSTMAN → API-ТЕСТИРОВАНИЕ
3.1.# Подготовка
☑ Создал запрос POST https://stavagro.com/php/calc.php
☑ Body → x-www-form-urlencoded
☑ Добавил поля из Payload
3.2.# Тест 1: false/false + пустые поля
☑ Отправил: technical=false, service=false
☑ name, phone, email — пустые
☑ Ответ: 200 OK
☑ Response: 1
☑ Результат: FAIL
3.3#. Тест 2: true/true + пустые поля
☑ Отправил: technical=true, service=true
☑ name, phone, email — пустые
☑ Ответ: 200 OK
☑ Response: 1
☑ Результат: FAIL

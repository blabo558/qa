### 1. Открытие и осмотр сайта

- [x] Главная страница открывается без ошибок
- [x] Контент отображается (блоки «Сервис», «О нас»)
- [x] Текст читаемый
- [x] Найдена кнопка «Оставить заявку на сервис»

### 2. DevTools → Network

- [x] Открыт DevTools (F12)
- [x] Вкладка Network работает
- [x] Фильтр Fetch/XHR применён
- [x] Keep log включён
- [x] Найден запрос `calc.php` (POST)
- [x] URL: `https://stavagro.com/php/calc.php`
- [x] Метод: POST
- [x] Формат: `x-www-form-urlencoded`
- [x] Headers просмотрены
- [x] Payload просмотрен (`technical`, `service`, `name`, `phone`, `email`)
- [x] Response просмотрен (`1`)

### 3. Postman → API-тестирование

**Тест 1: `false/false` + пустые поля**
- [x] Отправлен запрос с `technical=false, service=false`
- [x] `name`, `phone`, `email` — пустые
- [x] Ответ: `200 OK`
- [x] Response: `1`
- [x] Результат: ❌ **FAIL**

**Тест 2: `true/true` + пустые поля**
- [x] Отправлен запрос с `technical=true, service=true`
- [x] `name`, `phone`, `email` — пустые
- [x] Ответ: `200 OK`
- [x] Response: `1`
- [x] Результат: ❌ **FAIL**

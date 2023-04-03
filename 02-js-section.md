# Раздел 2: JS core

> Пишите код так, как будто сопровождать его будет склонный к насилию психопат, который знает, где вы живёте — Джон Ф. Вудс

### Блок 2.1: Основы веба и HTTP

Изучим один из самых важных протоколов веба - HTTP. 
Вам, как фронтэндерам, необходимо понимать:
1) Как ваше клиенсткое приложение работает с сервером
2) Где и в каком виде можно передавать данные, использование расспространненных заголовков
3) Как тестировать и отлаживать серверное API (Postman / Chrome Dev Tools)

https://stepik.org/lesson/14823  
https://stepik.org/lesson/14824  
Остальное ищем сами

#### Задание 1:

Вам нужно попрактиковаться в использовнии API. Для отправки http запросов будем использовать
такой инструмент, как Postman
URL для запросов состоит из базового URL и пути для конретного эндпоинта.  
То, в каком виде должен быть запрос - указано в документации.  
Формат данных в запросе - JSON, если не знакомы с этим форматом - почитайте.  

API для тренировки будем использовать [отсбда](https://jsonplaceholder.typicode.com)  

1) Качаем [Postman](https://www.getpostman.com/), дальше все запросы отправляем с его помощью
2) Смотрим документацию к API
3) Пробуем получить данные через постмен

#### Задание 2:
Изучить xhr запросы на [сайте](https://demo.realworld.io) с помощью вкладки Network в Chrome Dev Tools
Пройдите процесс регистрации, посмотрите формат ошибок на некорректно-заполненные поля

#### Доп информация:
- [Принципы работы веба](https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/How_the_Web_works)
- [Что на самом деле происходит, когда пользователь вбивает в браузер адрес google.com](https://habr.com/ru/company/htmlacademy/blog/254825/) (Ознакомительно, нам интересны 3+ пункты, в работу TCP/IP и сокетов не углубляемся. Кстати, частый вопрос на собеседованиях.)
- [Что такое API](https://www.andreyolegovich.ru/PC/testing/api_testing.php)
- [Обзор протокола HTTP](https://developer.mozilla.org/ru/docs/Web/HTTP/Overview)
- [Что такое DNS](https://selectel.ru/blog/dns-server/)
- [REST для фронтэндера](https://ymatuhin.ru/front-end/restful_api_for_frontender/)
- [Понимание REST](http://spring-projects.ru/understanding/rest/)
- [REST простым языком](https://medium.com/@andr.ivas12/rest-%D0%BF%D1%80%D0%BE%D1%81%D1%82%D1%8B%D0%BC-%D1%8F%D0%B7%D1%8B%D0%BA%D0%BE%D0%BC-90a0bca0bc78)

#### Темы для ревью:
- Что такое DNS
- HTTP: что из себя представляет, структура запросов/ответов
- Методы запроса - GET/POST/PUT/DELETE
- Коды ответа (200, 201, 204, 301, 302, 40x, 500)
- Заголовки авторизации и Cookies, сессии на куках
- Структура url - path, query string, fragment
- REST API: что такое ресурс, ограничения, идемпотентность, кэширование

### Блок 2.2: Основы JS + Функции

Гуглим как установить Node.js и запустить js файл.   
[Знакомство с функциями](https://learn.javascript.ru/function-basics)  
[Function-expressions](https://learn.javascript.ru/function-expressions)
[Arrow-functions](https://learn.javascript.ru/arrow-functions-basics)  
[Массивы](https://learn.javascript.ru/array)  
[Методы примитивов](https://learn.javascript.ru/primitives-methods)

#### Внимание:
- Если материал показался вам не понятен - ищем в других источниках. В полиморфизм, диспетчеризацию и остальной computer science не углубляемся.
- В файловой структуре есть папка `__tests__`, где можно посмотреть проверки для вашего решения

#### Доп. материалы:
- [Числа](https://learn.javascript.ru/number)
- [var, let и const](https://medium.com/nuances-of-programming/%D0%B2-%D1%87%D1%91%D0%BC-%D1%80%D0%B0%D0%B7%D0%BD%D0%B8%D1%86%D0%B0-%D0%BC%D0%B5%D0%B6%D0%B4%D1%83-var-let-%D0%B8-const-%D0%B2-javascript-3084bfe9f7a3)
- [Функции](https://learn.javascript.ru/es-function)
- [Шаблон раннего возврата](http://gearmobile.github.io/javascript/early-return/)

#### Темы для ревью:
- Хранение чисел, неточные вычисления
- Ошибки
- Рекурсия
- Замыкания и область видимости
- Различия var/let/const, hoisting
- Модули / экспорты
- Побочные эффекты, чистота функций
- Guard Expression / ранний возврат
- Значения по умолчанию
- Функции высшего порядка
- Отличия стрелочных функций от обычных
- map / filter / reduce / forEach / find / flat / includes / indexOf / join / slice / splice / sort

#### Задание
Решаем задачки по очереди и учимся разбивать код на отдельные функции, называем переменные понятными именами, следим за отступами.

- [Hello Word!](https://codesandbox.io/s/hello-world-forked-knm77f)
- [Лазанья](https://codesandbox.io/s/sochnaya-lazanya-mayka-forked-u13fr4)
- [Спасение из темницы](https://codesandbox.io/s/inspiring-river-n98ne1)
- [Калькулятор стоимости услуг](https://codesandbox.io/s/kalkulyator-stoimosti-uslug-04-forked-qt2tev)
- [Правила посещения Поэтического клуба](https://codesandbox.io/s/pravila-poseshcheniya-poeticheskogo-kluba-forked-n7l7cu)
- [Чары Элиз](https://codesandbox.io/s/chary-eliz-06-forked-uymziq)
- [Покупка автомобиля](https://codesandbox.io/s/pokupka-avtomobilya-07-forked-xj61iu)
- [Наблюдение за птицами](https://codesandbox.io/s/08-nablyudenie-za-pticami-forked-gwchsx)
- [Смешанные соки](https://codesandbox.io/s/09-smeshannye-soki-forked-ryozoy?file=/src/index.js)
- [Доска рекордов](https://codesandbox.io/s/10-doska-rekordov-forked-yn4so6)
- [Парк аттракционов](https://codesandbox.io/s/11-park-attrakcionov-forked-uts62f)
- [Счастливые числа](https://codesandbox.io/s/12-schastlivye-chisla-forked-q2b66w)
- [Мастер Лазаньи](https://codesandbox.io/s/13-master-lazani-forked-6cwyek)
  
Дальше перехоим к [этим](https://github.com/mbelsky/js-problems/tree/master/problems) задачкам.
Используем методы массивов по максимуму.

### Блок 12: Классы + Коллекции
[ООП](https://habr.com/ru/company/ruvds/blog/665290/)  
[Классы](https://learn.javascript.ru/classes)  
[Коллекции](https://developer.mozilla.org/ru/docs/Web/JavaScript/Guide/Keyed_collections) 

#### Доп материалы:
- [Объекты (Кантор)](https://learn.javascript.ru/object)  
- [Методы объекта (Кантор)](https://learn.javascript.ru/object-methods)  
- [Статические свойства (Кантор)](https://learn.javascript.ru/static-properties-methods)  

#### Задание
Практикуемся в работе с объектами
- [10 задачек на объекты](https://github.com/emel93/JS_core/blob/main/tasks-object.md)
- [Создание классов](http://old.code.mu/tasks/javascript/oop/osnovy-raboty-s-oop-v-javascript.html)
- [Наследование](http://old.code.mu/tasks/javascript/oop/nasledovanie-klassov-v-javascript.html)

#### Темы для ревью:
- Методы объекта
- Классы: конструктор, методы, свойства, get/set, статические методы
- Map, Set
- rest, spread, destructuring
- Мемоизация

### Блок 13: Прототипы + Обработка ошибок
[Прототипы](https://learn.javascript.ru/prototypes)  
[Обработка исключений (видео)](https://www.youtube.com/watch?v=DwZ5TUULi2s)  
[Обработка ошибок (Кантор)](https://learn.javascript.ru/try-catch)  
[Пользовательские ошибки (Кантор)](https://learn.javascript.ru/custom-errors)  


#### Доп информация:
- [Привязка контекста (Кантор)](https://learn.javascript.ru/bind)
- [Стрелочные функции (Кантор)](https://learn.javascript.ru/arrow-functions)
- [instanceof (Кантор)](https://learn.javascript.ru/instanceof)
- [Подробно о методах apply(), call() и bind()](https://medium.com/@stasonmars/%D0%BF%D0%BE%D0%B4%D1%80%D0%BE%D0%B1%D0%BD%D0%BE-%D0%BE-%D0%BC%D0%B5%D1%82%D0%BE%D0%B4%D0%B0%D1%85-apply-call-%D0%B8-bind-%D0%BD%D0%B5%D0%BE%D0%B1%D1%85%D0%BE%D0%B4%D0%B8%D0%BC%D1%8B%D1%85-%D0%BA%D0%B0%D0%B6%D0%B4%D0%BE%D0%BC%D1%83-javascript-%D1%80%D0%B0%D0%B7%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%87%D0%B8%D0%BA%D1%83-ddd5f9b06290)


#### Темы для ревью:
- Наследование в классах
- Прототипная модель
- this
- Call / Apply, заимствование метода
- Потеря контекста, bind
- Отличия стрелочных функций от обычных
- throw/try/catch

### Блок 14: Асинхронное программирование + DOM API
[Асинхронное программирование](https://habr.com/ru/post/651037)  
[DOM](https://learn.javascript.ru/dom-nodes)  
[DOM API](https://developer.mozilla.org/ru/docs/Web/API/Document_Object_Model)

#### Доп информация:
- [Промисы (Кантор)](https://learn.javascript.ru/promise-basics)
- [Async/await (Кантор)](https://learn.javascript.ru/async-await)
- [Про цикл событий в JavaScript или "как на самом деле работает асинхронность"?](https://www.youtube.com/watch?v=8cV4ZvHXQL4)
- [Jake Archibald: все что я знаю про Event Loop в JavaScript](https://www.youtube.com/watch?v=j4_9BZezSUA)
- [Полное понимание синхронного и асинхронного JavaScript с Async/Await](https://medium.com/@stasonmars/%D0%BF%D0%BE%D0%BB%D0%BD%D0%BE%D0%B5-%D0%BF%D0%BE%D0%BD%D0%B8%D0%BC%D0%B0%D0%BD%D0%B8%D0%B5-%D1%81%D0%B8%D0%BD%D1%85%D1%80%D0%BE%D0%BD%D0%BD%D0%BE%D0%B3%D0%BE-%D0%B8-%D0%B0%D1%81%D0%B8%D0%BD%D1%85%D1%80%D0%BE%D0%BD%D0%BD%D0%BE%D0%B3%D0%BE-javascript-%D1%81-async-await-ba5f47f4436)
- [Хранение данные](https://learn.javascript.ru/data-storage) (IndexedDB - просто знайте, что такая штука есть)
- [События](https://learn.javascript.ru/events)

#### Темы для ревью:
- стек вызовов
- таймеры
- event loop
- callback
- Promise
- async / await
- Модель событий в js. Capturing / Bubbling.
- fetch
- LocalStorage / Cookies
- Полифиллы

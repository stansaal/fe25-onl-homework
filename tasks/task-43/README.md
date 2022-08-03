# Задание 43 - Запросы к API

Задание к занятию 46, 49, 50.

## Цель
- Научиться общаться с сервером посредством REST-API
- Познакомиться с библиотекой Axios
- Попрактиковать получение данных через GET запрос, научиться применять заголовки

## Что нужно сделать
Реализовать получение списка статей из [API](https://api.spaceflightnewsapi.net/v3/documentation#/Article/get_articles) - метод ```GET /articles``` и вывести его на главной странице

#### Детально:
1. [ ] Добавить в проект библиотеку [Axios](https://axios-http.com/)
2. [ ] Создать в отдельном каталоге ```src/api``` модуль для запросов к API. Файл ```src/api/index.ts```. В нём создать [инстанс Axios](https://axios-http.com/docs/instance), в котором задать ```baseURL  https://api.spaceflightnewsapi.net/v3```. Этот адрес используется  для всех запросов к [API](https://api.spaceflightnewsapi.net/v3/documentation#/Article/get_articles).
3. [ ] В том же инстансе задать заголовок ```Content-Type: application/json```, указывающий на то, что мы отправляем запрос в формате JSON.
4. [ ] Используя полученый инстанс создать в отдельном модуле в каталоге ```src/api``` [асинхронную функцию](https://learn.javascript.ru/async-await) ```getArticles```, которая будет отправлять ```GET``` запрос по пути ```/articles``` и возвращать результат выполнения запроса - массив объектов-статей.
5. [ ] Для хранения списка статей создать в компоненте списка (прим. Featured.tsx и Recent.tsx) локальный стейт, используя хук ```useState```
6. [ ] Отправлять запрос на получение списка статей в момент монтирования компонента (используя хук useEffect). Полученный список сохранять в стейт.

## На что обратить внимание
1. При работе с запросами код работает асинхронно, необходимо владеть работой с [Promise](https://learn.javascript.ru/promise) и [async/await](https://learn.javascript.ru/async-await).
2. Все ошибки должны обрабатываться (нам пока достаточно выводить их в консоль). Используйте [try..catch](https://learn.javascript.ru/exception) в функции запроса в обязательном порядке.
3. Запросы и стейт [должны быть типизированы](https://bobbyhadz.com/blog/typescript-http-request-axios#making-http-get-requests-with-axios-in-typescript)
4. Запрос должен происходить только один раз при монтировании компонента. Повторите [хуки useState и useEffect](https://ru.reactjs.org/docs/hooks-overview.html)

## Что мне может в этом помочь
- [Документация Axios](https://axios-http.com/)
- [Документация по хукам React](https://ru.reactjs.org/docs/hooks-overview.html)
- [Promise](https://learn.javascript.ru/promise) и [async/await](https://learn.javascript.ru/async-await)
- [try..catch](https://learn.javascript.ru/exception)
- [Как типизировать запросы с Axios](https://bobbyhadz.com/blog/typescript-http-request-axios#making-http-get-requests-with-axios-in-typescript)
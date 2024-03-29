# 3 модуль - ReactJS - Домашнаяя работа

Выполнять домашнюю работу предлагается поэтапно, параллельно обучению с 39 по 52 занятие.\
Каждому занятию соответствует одно задание, которое публикуется после урока.\
Шаг за шагом вы разработаете полноценное frontend-приложение.

[Перейти к списку заданий](#задания)

#### Содержание
1. [Цель](#цель)
2. [Вводные данные](#вводные-данные)
3. [Требования](#требования)
4. [Сдача заданий](#сдача-заданий)
5. [Задания](#задания)

## Цель
1. Освоить основные методы библиотек React и Redux
2. Изучить на практике основы работы с REST API
3. Понять основные этапы разработки интерфейсов, от создания нового приложения до запуска на сервере.


## Вводные данные
Разрабатывать вам предстоит новостной ресурс про космос.\
Это небольшой сайт из трёх страниц:
- Список статей
- Страница статьи
- Страница "Об авторе"

### Вёрстка
Верстать ничего не нужно, сосредоточимся на работе с компонентами React.\
Для этого вам предоставлена готовая HTML вёрстка в этом репозитории.
> Обратите внимание, в вёрстке используются библиотеки [Bootstrap](https://getbootstrap.com) и [jQuery](https://jquery.com/).
> 
> **Bootstrap** даёт готовые **CSS классы**, их необходимо размещать в пропе ```className```.
> 
> **jQuery** - это **JS** библиотека, которая используется чтобы реализовывать небольшой интерактив. \
> Её в наше будущее приложение **НЕ импортируем**, и имеющийся готовый JS код **НЕ используем**. \
> Весь функционал приложения мы будем реализовывать сами на React. 

Чтобы скачать вёрстку себе на компьютер - склонируйте этот репозиторий.
```
git clone https://github.com/stansaal/fe25-onl-homework.git
```

### API
В процессе разработки новостного ресурса вам потребуется брать откуда-то новости. \
Мы научимся взаимодействовать с **REST API**, и в качестве примера используем открытый [API с новостями про космос](https://thespacedevs.com/snapi). \
На выбор там представлено 4 разных API, выбирайте любой.

Нам понадобится только ссылка на метод и документация. Например:
> API endpoint: [https://api.spaceflightnewsapi.net/v3/articles](https://api.spaceflightnewsapi.net/v3/articles) \
> [Документация](https://api.spaceflightnewsapi.net/v3/documentation#/Article)

### Create React App
Приложение создавайте сами с нуля. \
Самый простой способ, с которым вы уже знакомы, это CRA (Create React App).

Чтобы создать приложение выполните:
```
npx create-react-app my-space-news-app --template typescript

или

yarn create react-app my-space-news-app --template typescript

```
Обратите внимание на использование [TypeScript](https://www.typescriptlang.org/) в приложении. Типизируйте компоненты!

## Требования
1. Приложение должно использовать библиотеку [React.js](https://ru.reactjs.org/)
2. Глобальное состояние должно быть реализовано с помощью [Redux](https://redux.js.org/)
3. Код должен быть строго типизирован с помощью [TypeScript](https://www.typescriptlang.org/)
4. Допускается использование библиотеки [Axios](https://axios-http.com/docs/intro) для запросов
5. НЕ допускается использование сторонних библиотек UI компонентов, таких как MUI или AntD и подобных

## Сдача заданий
1. Код приложения публикуйте в открытом репозитории на GitHub.
2. Ссылку на репозиторий отправляйте в личные сообщения мне [@stansaal](https://t.me/stansaal). Добавьте меня в репозиторий.
3. Для каждого задания создавайте новую ветку от ```master``` с номером задания. Например ```task-39```. \
Для этого выполните ```git checkout master && git checkout -b task-39```
4. По завершению задания создавайте коммит с описанием того, что выполнили. И отправляйте ветку в GitHub.
```
git commit -m "task-39: Создал компонент Template"
git push -u origin task-39
```
5. Создавайте Pull Request этой ветки в ```master```, отмечайте меня как Reviewer в PR.
6. После проверки задания я оставлю комментарий, либо приму PR и ветка с заданием сольётся в ```master```. Тогда задание принято.

## Задания
1. [Задание 0](tasks/task-0/) - Создание репозитория
2. [Задание 41](tasks/task-41/) - Композиция компонентов
3. [Задание 42](tasks/task-42/) - Навигация в приложении
4. [Задание 43](tasks/task-43/) - Запросы к API
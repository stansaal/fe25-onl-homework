# Задание 42 - Навигация сайта

Задание к занятию 42.

## Цель
- Познакомиться с библиотекой react-router-dom, изучить основные компоненты и хуки этой библиотеки
- Понять, как реализуется маршрутизация в React-приложениях

## Что нужно сделать
Реализовать маршрутизацию и навигацию по сайту между тремя существующими страницами

#### Детально:
1. [ ] Создать роуты под необходимые страницы. \
- Главная - /
- Статья - /post/:id
- Автор - /author/:id
2. [ ] Реализовать переход на эти страницы по навигации в шапке сайта.
3. [ ] Реализовать переход на страницу статьи по нажатию на заголовок или картинку в карточке статьи. \
- С карточек статьи на любой странице - главной, автора или статьи.
- Ссылка на статью должна формироваться с ID статьи. (прим. /post/321)
4. [ ] Реализовать переход на страницу автора по нажатию на аватар или имя автора в карточке статьи.
- Ссылка на автора должна формироваться с ID автора.
5. [ ] На странице статьи необходимо получать ID статьи из адресной строки и выводить рядом с заголовком через шаблонную строку.

## На что обратить внимание
1. Адреса должны быть в нижнем регистре, заместо пробелов - дефис (-)
2. Переход между всеми страницами должен выполняться без перезагрузки страницы.
3. При перезагрузке страницы, пользователь должен оставаться там же, где и находился.
4. Возможно использовать как react-router-dom [5 версии](https://v5.reactrouter.com/web/guides/quick-start), так и [6 версии](https://reactrouter.com/). В них есть отличия.

## Что мне может в этом помочь
- [Документация React Router Dom v5](https://v5.reactrouter.com/web/guides/quick-start)
- [Документация React Router Dom v6](https://reactrouter.com/)
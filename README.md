## TODO

### High Priority

- [x] Validate html
- [ ] Uploud to github

### Low Priority

- [ ] use chechlist to validite

# My Project

This is a sample project that demonstrates basics of HTML and CSS, based on BEM approach.
See \*.css files in common.blocks folder.

Files structure:

```
.
├── README.md
├── checklist-1.pdf
├── common.blocks --> CSS block files according to BEM
│   ├── description.css
│   ├── digits.css
│   ├── feynman.css
│   ├── footer.css
│   ├── header.css
│   ├── kaufman.css
│   ├── logo.css
│   ├── page.css
│   ├── section-subtitle.css
│   ├── section-title.css
│   ├── table.css
│   ├── two-columns.css
│   └── unknown.css --> добавил сюда блоки по логике пока не понятные
├── images
│   ├── facebook_color_white.svg
│   ├── feynman.png
│   ├── instagram_color_white.svg
│   ├── kaufman-triangle.svg
│   ├── logo_place_footer.svg
│   ├── logo_place_header.svg
│   ├── two_again.png
│   └── vk_color_white.svg
├── index.html
├── styles
│   ├── normalize.css
│   └── style.css --> not used
├── texts.md
└── tree.md
```

## Getting Started

Use git clone to get copy of the project.

### Prerequisites

Live server vscode extension to run project locally.
EditorConfig vscode extension to format code. See .editorconfig

### Installing

Step by step instructions on how to install the project

1. Clone the repository
2. Start the server

## Usage

open 127.0.0.1 port 5500 locally

## Contributing

None

## License

This project is licensed under the MIT License

## Contact

- Email: dev.miroshnikov.m@ya.ru

## Commments

"БЭМ не рекомендует общие ресеты.
Блок — независимый от окружения компонент. Он не может рассчитывать на то, что стили сброшены какими-то внешними по отношению к блоку средствами"

You should reset CSS on block level.

Page structure:

Pseudocode:

```
div class="page"
  header class="header" -> reset CSS
  main class="content
    section class="digits -> reset CSS
    section class="feynman" -> reset CSS
    section class="kaufman" -> reset CSS
  footer class="footer" -> reset CSS
```

reset CSS:

```
  margin: 0;
  padding: 0;
  border-box - надо указывать?


```

## Questions

#В футере есть ссылки? По ним можно кликнуть?
вот так "#" можно ссылку оставить?

#У всех изображений есть атрибут alt ?
иконки считаются изображениями? на них надо делать alt?

#Обнулены ли стандартные значения отступов у элементов (заголовков, параграфов, списков) в соответствии с брифом?
см Сomments выше

#Для создания сеток используется flex либо grid-layout ?
а что надо использовать?

#У блоков фиксированная высота? Растягивается ли блок, когда текст внутри него увеличивается в 2–3 раза?
а как надо? блок должен растягиваться?
в feynman\_\_subtitle не указаны размеры блока.

#Нет ли на странице скрытых с помощью CSS заголовков?
имеется в виду атрибут CSS hidden?

# Cheklict

## Общее

- [ ] Репозиторий содержит все необходимые файлы: изображения, файлы стилей и HTML?
- [ ] Стили подключены отдельным файлом? Подключён ли в head файл normalize.css ?
- [ ] Соответствует ли вёрстка брифу внешне?
- [ ] В коде HTML и CSS нет опечаток? Страница валидна? Рекомендуем использовать валидатор разметки от w3.org
- [ ] Все блоки из брифа свёрстаны?
- [ ] Все блоки, элементы и модификаторы названы в соответствии с брифом?
- [ ] Названия классов CSS в разметке соответствуют явно указанным в брифе?
- [ ] Добавлены ли в футер иконки и текст?
- [ ] В футере есть ссылки? По ним можно кликнуть?

## Семантика

- [ ] У всех изображений есть атрибут alt ?
- [ ] Для вёрстки заголовков применяются несколько тегов от <h1> до <h6> , текстовые блоки размечены тегами
<p> , присутствуют элементы <header> , <main> , <footer> , <section> ? Они используются по назначению?

## Заголовки

- [ ] На странице есть заголовок первого уровня? Соответствуют ли заголовки иерархии страницы? Нет ли на
      странице скрытых с помощью CSS заголовков?

## CSS

- [ ] Соответствуют ли брифу значения отступов у элементов?
- [ ] Обнулены ли стандартные значения отступов у элементов (заголовков, параграфов, списков) в соответствии с брифом?
- [ ] Картинки в проекте не перекрывают текст? Текст располагается над изображением по оси Z?
- [ ] Абсолютное позиционирование применено только к тем элементам, о которых сказано в брифе?
- [ ] У всех ли абсолютно спозиционированных элементов заданы координаты по двум осям (например, top и left )?
- [ ] У блоков фиксированная высота? Растягивается ли блок, когда текст внутри него увеличивается в 2–3 раза?
- [ ] Ссылки, фоны секций и шрифты раскрашены как в брифе?
- [ ] Для создания сеток используется flex либо grid-layout ?

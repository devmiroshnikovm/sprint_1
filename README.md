## TODO

### High Priority

- [x] Validate html
- [ ] Uploud to github

### Low Priority

- [ ] use chechlist to validite

# My Project

This is a sample project that demonstrates basics of HTML and CSS, based on BEM approach.
See \*.css files in common.blocks folder.

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

"БЭМ не рекомендует общие ресеты
Блок — независимый от окружения компонент. Он не может рассчитывать на то, что стили сброшены какими-то внешними по отношению к блоку средствами"

You should reset CSS on block level.

Page structure:

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


```

## Questions

#В футере есть ссылки? По ним можно кликнуть?
вот так можно ссылку оставить?

#У всех изображений есть атрибут alt ?
иконки считаются изображениями? на них надо делать alt?

#Обнулены ли стандартные значения отступов у элементов (заголовков, параграфов, списков) в соответствии с брифом?
?

#Для создания сеток используется flex либо grid-layout ?
?

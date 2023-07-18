## About this extension

This package aims at providing a complete set of tools to start coding Nunjucks templates in VSCode.  
- Language configuration
- Syntax definition
- Snippets for every features listed in the [Nunjucks templating Documentation](https://mozilla.github.io/nunjucks/templating.html)

### Snippets

| Prefix      | HTML Snippet Content                             |
| ----------- | ------------------------------------------------ |
| `block`     | `{% block name %} {% endblock %}`                |
| `njk`       | `{% %}`                                          |
| `var`       | `{{ variable }}`                                 |
| `extends`   | `{% extends "template" %}`                       |
| `include`   | `{% include "template" %}`                       |
| `filter`    | `{% filter filter %} {% endfilter %}`            |
| `for`       | `{% for item in sequence %} {% endfor %}`        |
| `asyncEach` | `{% asyncEach item in sequence %} {% endeach %}` |
| `asyncAll`  | `{% asyncAll item in sequence %} {% endeach %}`  |
| `if`        | `{% if condition %} {% endif %}`                 |
| `ife`       | `if else`                                        |
| `ifel`      | `if elif`                                        |
| `elif`      | `elif`                                           |
| `else`      | `else`                                           |
| `end`       | `{% endif %}`                                    |
| `set`       | `set`                                            |
| `macro`     | `macro`                                          |
| `import`    | `import`                                         |
| `from`      | `from import`                                    |
| `raw`       | `raw`                                            |
| `call`      | `call`                                           |
| `var`       | `alt variable`                                   |
| `super`     | `super`                                          |
| `or`        | `or`                                             |
| `pipe`      | `pipe`                                           |

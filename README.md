## Nunjucks complete package for Visual Studio Code

This package aims at providing a complete package to start coding Nunjucks templates in VSCode :  
- Language configuration
- Syntax definition (forked from [ronnidc's package](https://marketplace.visualstudio.com/items?itemName=ronnidc.nunjucks))
- Snippets for every features listed in [Nunjucks templating documentation](https://mozilla.github.io/nunjucks/templating.html)
- Template formatter via [Nanda Okitavera's extension](https://marketplace.visualstudio.com/items?itemName=okitavera.vscode-nunjucks-formatter) which is automatically installed with this extension.   

-------

### Demo
![Demo](./docs/demo.gif)

### Snippets list

#### Basics  
| Prefix               | HTML Snippet Content                                       |
| -------------------- | ---------------------------------------------------------- |
| `comment`            | `{# comment #}`                                            |
| `cblock`             | `{# comment #}`                                            |
| `var, show, display` | `{{ var }}`                                                |
| `super`              | `{{ super() }}`                                            |

-------

#### Tags  
| Prefix               | HTML Snippet Content                                       |
| -------------------- | ---------------------------------------------------------- |
| `njk, tag`           | `{% %}`                                                    |
| `extends`            | `{% extends "template" %}\n$0`                             |
| `include`            | `{% include "template" %}\n$0`                             |
| `include_missing`    | `{% include "template" ignore missing %}`                  |
| `import`             | `{% import "template" as var with context %}`              |
| `from`               | `{% from "template" import "macro" as var with context %}` |
| `block`              | `{% block name %} {% endblock %}`                          |
| `if`                 | `{% if condition %} {% endif %}`                           |
| `ife`                | `if else`                                                  |
| `ifel`               | `if elif`                                                  |
| `ifelelse`           | `if elif else`                                             |
| `elif`               | `elif`                                                     |
| `else`               | `else`                                                     |
| `end`                | `{% endif %}`                                              |
| `for`                | `{% for item in sequence %} {% endfor %}`                  |
| `fori`               | `{% for index,value in sequence %} {% endfor %}`           |
| `set`                | `{% set var = "value" %}`                                  |
| `seto`               | `{% set var = { var: "value" } %}`                         |
| `setc`               | `{% set var %} content {% endset %}`                       |
| `macro`              | `{% macro name %} {% endmacro %}`                          |
| `call`               | `{% call macro %} {% endcall %}`                           |
| `caller`             | `{{ caller() }}`                                           |
| `raw`                | `{% raw %} {% endraw %}`                                   |
| `verbatim`           | `{% verbatim %} {% endverbatim %}`                         |
| `asyncEach`          | `{% asyncEach item in sequence %} {% endeach %}`           |
| `asyncAll`           | `{% asyncAll item in sequence %} {% endeach %}`            |

-------

#### Global functions  
| Prefix               | HTML Snippet Content                                       |
| -------------------- | ---------------------------------------------------------- |
| `rangef`             | `range(start, stop)`                                       |
| `rangesf`            | `range(start, stop, step)`                                 |
| `cyclf`              | `cycler(firstValue, secondValue)`                          |
| `joinerf`            | `joiner()`                                                 |

-------

#### Builtin Filters  
| Prefix               | HTML Snippet Content                                       |
| -------------------- | ---------------------------------------------------------- |
| `pipe`               | `\| `                                                      |
| `filter`             | `{% filter filter %} {% endfilter %}`                      |
| `defaultf`           | `\| default(value, fallback)`                              |
| `absf`               | `\| abs`                                                   |
| `batchf`             | `\| batch(number)`                                         |
| `capitalize`         | `\| capitalize`                                            |
| `dictf`              | `\| dictsort`                                              |
| `dumpf`              | `\| dump`                                                  |
| `escf`               | `\| escape`                                                |
| `forcescf`           | `\| escape`                                                |
| `firstf`             | `\| first`                                                 |
| `floatf`             | `\| float`                                                 |
| `groupf`             | `\| groupby`                                               |
| `indf`               | `\| indent(spaces)`                                        |
| `intf`               | `\| int`                                                   |
| `joinf`              | `\| join(separator)`                                       |
| `joinaf`             | `\| join(separator, indexKey)`                             |
| `lastf`              | `\| last`                                                  |
| `lf`                 | `\| length`                                                |
| `list`               | `\| list`                                                  |
| `lowf`               | `\| lower`                                                 |
| `nlf`                | `\| nl2br`                                                 |
| `randf`              | `\| random`                                                |
| `rejf`               | `\| reject()`                                              |
| `rejof`              | `\| reject(odd\|even)`                                     |
| `rejdf`              | `\| reject(divisibleby)`                                   |
| `rejattrf`           | `\| rejectattr(attr)`                                      |
| `repf`               | `\| replace(needle, haystack)`                             |
| `repof`              | `\| replace(needle, haystack, occurrence)`                 |
| `revf`               | `\| reverse`                                               |
| `roundf`             | `\| round(digit)`                                          |
| `safef`              | `\| safe`                                                  |
| `self`               | `\| select()`                                              |
| `selof`              | `\| select(odd\|even)`                                     |
| `seldf`              | `\| select(divisibleby)`                                   |
| `selattrf`           | `\| selectattr(attr)`                                      |
| `slicef`             | `\| slice(count)`                                          |
| `sortf`              | `\| sort(array, ?reverse, ?caseSentive, attr)`             |
| `strf`               | `\| string`                                                |
| `stripf`             | `\| striptags(?preserve_linebreaks)`                       |
| `titlef`             | `\| title`                                                 |
| `trimf`              | `\| trim`                                                  |
| `truncf`             | `\| truncate(?keep, replace)`                              |
| `upf`                | `\| upper`                                                 |
| `urlencf`            | `\| urlencode`                                             |
| `urlizef`            | `\| urlize`                                                |
| `urlizetf`           | `\| urlize(?keep, ?truncate)`                              |
| `wordf`              | `\| wordcount`                                             |

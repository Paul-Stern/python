+++
draft = false
outputs = "Reveal"
+++

## Занятие №2 {#занятие-2}

Переменные, выражения, инструкции

---


### Текстовый редактор {#текстовый-редактор}

-   <https://www.slant.co/topics/12/~best-programming-text-editors>
-   <https://insights.stackoverflow.com/survey/2019#development-environments-and-tools>
-   <https://github.com/collections/text-editors>

---

-   VS Code
-   Atom
-   Emacs
-   Vim

---


### Значения, выражения и инструкции {#значения-выражения-и-инструкции}

**Структура кода:**

инструкции

↑

выражения

↑

значения, переменные и операторы

---


### Документация {#документация}

<https://docs.python.org/3/index.html>

Главные разделы:

-   What's new
-   Library Reference
-   Language Reference

---


### Значения {#значения}

<https://docs.python.org/3/reference/datamodel.html#objects-values-and-types>

> An object’s type &hellip; defines the possible values for objects of that type.

<!--quoteend-->

> The value of some objects can change.

---


### Выражения {#выражения}

<https://docs.python.org/3/reference/expressions.html>

---


### Инструкции {#инструкции}

<https://docs.python.org/3/reference/simple%5Fstmts.html#simple-statements>

---


### Инструкция присваивания (assignment statement) {#инструкция-присваивания--assignment-statement}

<https://docs.python.org/3/reference/simple%5Fstmts.html#assignment-statements>

Инструкция присваивания создает переменную и _присваивает_ ей значение.

`имя_переменной = значение`

По правилам составления имен см. PEP8.

---

```python
help_message = 'Если Вы хотите прервать выполнение программы, '
	       + 'то нажмите Ctrl-C'
height = 10
width = 5.5
```

---


### PEPs {#peps}

PEP &mdash; Python Enhancement Proposal.
<https://www.python.org/dev/peps/>

<https://realpython.com/python-pep8/>

-   <https://pep8.org/#descriptive-naming-styles>
-   <https://pep8.org/#global-variable-names>

---


### (Не)интеркативный режим {#не--интеркативный-режим}

---

Введите в консоли:

```python
10
```

Получите ли Вы что-то в ответ? Если да, то что?

Напишите то же самое в скрипте. Будет ли результат таким же?

_Для корректной работы скрипта в его конец необходимо добавить:_

```python
input("Нажмите Enter, чтобы выйти")
```

---


### Приоритет операторов {#приоритет-операторов}

`()`    **>**    `**`    **>**    `*` `/`    **>**    `+` &minus;

---


### Комментарии {#комментарии}

---


### Отладка {#отладка}

-   Syntax error
-   Runtime error
-   Semantic error

---


### Дополнительно {#дополнительно}

-   `dir()`
-   `help()`
-   Standard Library

+++
draft = false
outputs = "Reveal"
+++

## Основы программирования на языке Python {#основы-программирования-на-языке-python}

---


### Занятие № 1 {#занятие-1}

Общие сведения и инструменты разработки

---

Видели ли Вы код на Python?

---

Фрагмент random.py:

```python
def triangular(self, low=0.0, high=1.0, mode=None):
    """Triangular distribution.

    Continuous distribution bounded by given lower and upper limits,
    and having a given mode value in-between.

    http://en.wikipedia.org/wiki/Triangular_distribution

    """
    u = self.random()
    try:
	c = 0.5 if mode is None else (mode - low) / (high - low)
    except ZeroDivisionError:
	return low
    if u > c:
	u = 1.0 - u
	c = 1.0 - c
	low, high = high, low
    return low + (high - low) * (u * c) ** 0.5
```

---

Код может выглядеть по-разному.

---

Фрагмент filedialog.py:

```python
class Directory(commondialog.Dialog):
    "Ask for a directory"

    command = "tk_chooseDirectory"

    def _fixresult(self, widget, result):
	if result:
	    # convert Tcl path objects to strings
	    try:
		result = result.string
	    except AttributeError:
		# it already is a string
		pass
	    # keep directory until next time
	    self.options["initialdir"] = result
	self.directory = result # compatibility
	return result
```

---

В чем разница между этими двумя блоками кода?

---

Что такое программирование?

---

В общем смысле, это способ взаимодействия с компьютером.

---

Какие знания и умения необходимы для овладения программированием?

---

-   Математические знания
-   Владение навыками алгоритмического мышления
-   Владение ИКТ
    -   Компьютером
    -   Интернетом
-   Владение английским языком

---


#### Языки программирования {#языки-программирования}

---

Какими бывают языки программирования? На какие 2 группы их можно поделить?

---

Языки программирования:

-   компилируемые
-   интерпретируемые

---

Компилируемые языки:

Исходный код → исполняемый код → исполнение

Среди них:

-   C
-   C++
-   Go
-   Rust

---

Интерпретируемые языки:

Исходный код → исполнение (интерпретатором)

Среди них:

-   JavaScript
-   Bash
-   PHP

---

Как вы думаете, к каким относится Python?

---

Python &mdash; интерпретируемый язык

---

Короткие программы на интерпретируемых языках называют _скриптами_

---


#### Эволюция языка {#эволюция-языка}

Версии языка

---

Зачем выпускать новые версии языка?

---

Чтобы:

-   исправить ошибки
-   улучшить производительность
-   обогатить язык средствами выразительности

---

-   0.9.0 &mdash; 1991
-   1.0 &mdash; 1994
-   2.0 &mdash; 2000
    -   2.1 &mdash; 2001
    -   &hellip;
    -   2.7 &mdash; 2010
        -   &hellip;
        -   2.7.16 &mdash; 2019

---

-   3.0 &mdash; 2008
-   &hellip;
-   3.7 &mdash; 2018
-   3.7.4 &mdash; 2019

---

Заметили что-нибудь необычное?

---

Почему версии 2.7+ и 3+ существуют параллельно?

---


#### Рейтинг языка {#рейтинг-языка}

Python входит в пятерку лучших языков по разным рейтингам, например, [TIOBE](https://www.tiobe.com/tiobe-index/) и [StackOverflow](https://insights.stackoverflow.com/survey/2018/#most-loved-dreaded-and-wanted).

---

С чем это может быть связано?

---


#### The Zen of Python (выдержка) {#the-zen-of-python--выдержка}

1.  Beautiful is better than ugly.
2.  Explicit is better than implicit.
3.  Simple is better than complex.
4.  Complex is better than complicated.
5.  &hellip;
6.  &hellip;
7.  Readability counts.

&hellip;

---


#### Инструменты разработки {#инструменты-разработки}

-   Интерпретатор
    -   Python
    -   IPython
-   Текстовый редактор

    -   IDLE
    -   Emacs / Vim
    -   VSCode

    Jupyter Notebooks

---


#### Установка Python {#установка-python}

Текущую версию языка для 64-битного Windows можно найти по ссылке: <https://www.python.org/ftp/python/3.7.4/python-3.7.4-amd64.exe>

Другие платформы: <https://www.python.org/downloads/release/python-374/>

---

Приступим!

---


#### Примеры программ {#примеры-программ}

```python
print('x * 4 =', int(input('x = ')) * 4)
```

---

```python
print('Первый отрезок + 4см = ', int(input('Первый отрезок = (в см) ')) + 4, 'см')
```

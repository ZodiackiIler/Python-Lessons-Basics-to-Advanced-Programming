## Урок 3: Модули и пакеты

В этом уроке мы рассмотрим модули и пакеты в языке программирования Python. Модули позволяют организовать код в отдельные файлы для повторного использования, а пакеты объединяют несколько модулей в иерархическую структуру.

Часть 1: Создание и использование модулей

Модуль - это файл, содержащий код на языке Python. Модули используются для организации кода в логические блоки и обеспечивают повторное использование. Модули могут содержать функции, переменные, классы и другие элементы кода.

Пример: Создание модуля

Создайте новый файл с расширением `.py` (например, `my_module.py`) и определите в нем функции или переменные:

<img src="https://github.com/ZodiackiIler/Python-Lessons-Basics-to-Advanced-Programming/blob/main/lesson3/module0.png">

```python
# my_module.py
def greet(name):
    print("Привет, " + name + "!")

def add_numbers(x, y):
    return x + y
```

Чтобы использовать модуль, его нужно импортировать в другой файл с помощью ключевого слова `import`. Затем вы можете использовать функции и переменные модуля в этом файле.

Пример: Использование модуля

```python
import my_module

my_module.greet("Анна")

result = my_module.add_numbers(3, 5)
print(result)
```
<img src="https://github.com/ZodiackiIler/Python-Lessons-Basics-to-Advanced-Programming/blob/main/lesson3/module1.png">

В этом примере модуль `my_module` импортируется с помощью ключевого слова `import`. Затем мы можем использовать функции `greet` и `add_numbers` из модуля.

Часть 2: Работа с внешними модулями и библиотеками

В Python существует огромное количество внешних модулей и библиотек, которые расширяют функциональность языка и предоставляют готовые решения для различных задач. Чтобы использовать внешний модуль или библиотеку, их необходимо установить и импортировать в свой код.

Пример: Установка и использование внешней библиотеки

1. Установите библиотеку с помощью менеджера пакетов, например, `pip`. В командной строке выполните:

```
pip install название_библиотеки
```

2. Импортируйте библиотеку в свой код:

```python
import название_библиотеки

# Использование функций или классов из библиотеки
название_библиотеки.функция()
```

В этом примере мы устанавливаем внешнюю библиотеку с помощью `pip` и затем импортируем ее в свой код. Мы можем использовать функции или классы из библиотеки, указывая их имя и вызывая их методы или функции.

Модули и библиотеки предоставляют мощные инструменты для организации кода, повторного использования и расширения функциональности языка Python. При необходимости вы можете создавать собственные модули или использовать внешние модули и библиотеки для более эффективной разработки программ.

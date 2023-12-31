## Урок 4: Работа с файлами

В этом уроке мы рассмотрим работу с файлами в языке программирования Python. Вы научитесь открывать файлы, читать данные из файлов, записывать данные в файлы и обрабатывать файловый ввод-вывод.

Часть 1: Чтение данных из файлов

Для чтения данных из файла сначала нужно открыть его с помощью функции `open()`. Указывается имя файла и режим доступа (например, "r" для чтения). Затем можно использовать методы чтения, такие как `read()`, `readline()` или `readlines()` для получения содержимого файла.

Пример: Чтение данных из файла

```python
file = open("file.txt", "r")
content = file.read()
print(content)
file.close()
```

В этом примере мы открываем файл `file.txt` для чтения. Затем с помощью метода `read()` мы получаем содержимое файла и сохраняем его в переменной `content`. После чтения файла его следует закрыть с помощью метода `close()`.

Часть 2: Запись данных в файлы

Для записи данных в файл нужно открыть его в режиме записи ("w" или "a") с помощью функции `open()`. Затем можно использовать методы записи, такие как `write()` или `writelines()`, чтобы записать данные в файл.

Пример: Запись данных в файл

```python
file = open("file.txt", "w")
file.write("Привет, мир!")
file.close()
```

В этом примере мы открываем файл `file.txt` в режиме записи. Затем с помощью метода `write()` мы записываем строку "Привет, мир!" в файл. После записи данных файл следует закрыть с помощью метода `close()`.

Часть 3: Обработка файлового ввода-вывода

Для удобной работы с файлами можно использовать оператор `with`, который автоматически закрывает файл после окончания его использования. В блоке `with` можно выполнять операции чтения или записи данных в файл.

Пример: Обработка файлового ввода-вывода с использованием оператора `with`

```python
with open("file.txt", "r") as file:
    content = file.read()
    print(content)
```

В этом примере файл `file.txt` открывается в режиме чтения с помощью оператора `with`. В блоке `with` мы читаем содержимое файла и выводим его на экран. После выхода из блока `with` файл автоматически закрывается, даже если возникнут исключения.

Работа с файлами является важной частью программирования, поскольку позволяет сохранять и извлекать данные из файлового хранилища. Python предоставляет удобные инструменты для работы с файлами, что делает их обработку более эффективной и удобной.

---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.drawing/picturecollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, stream) {#int-int-io.RawIOBase}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, stream):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| stream | io.RawIOBase | Потоковый объект, содержащий данные изображения.|

###  Пример

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs)

```


##  add(upper_left_row, upper_left_column, file_name) {#int-int-str}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, file_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| file_name | str | Имя файла изображения.|

###  Пример

```python

# add a picture
pictures.add(1, 1, "image.jpg")

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| lower_right_row | int | Нижний индекс правой строки|
| lower_right_column | int | Индекс нижнего правого столбца|
| stream | io.RawIOBase | Потоковый объект, содержащий данные изображения.|

###  Пример

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, 5, 5, fs)

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name) {#int-int-int-int-str}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| lower_right_row | int | Нижний индекс правой строки|
| lower_right_column | int | Индекс нижнего правого столбца|
| file_name | str | Имя файла изображения.|

###  Пример

```python

# add a picture
pictures.add(1, 1, 5, 5, "image.jpg")

```


##  add(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| stream | io.RawIOBase | Потоковый объект, содержащий данные изображения.|
| width_scale | int | Масштаб ширины изображения в процентах.|
| height_scale | int | Масштаб высоты изображения в процентах.|

###  Пример

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs, 50, 50)

```


##  add(upper_left_row, upper_left_column, file_name, width_scale, height_scale) {#int-int-str-int-int}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| file_name | str | Имя файла изображения.|
| width_scale | int | Масштаб ширины изображения в процентах.|
| height_scale | int | Масштаб высоты изображения в процентах.|

###  Пример

```python

# add a picture
pictures.add(1, 1, "image.jpg", 50, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
* класс [PictureCollection](/cells/ru/python-net/aspose.cells.drawing/picturecollection)

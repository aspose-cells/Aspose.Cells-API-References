---
title: add_picture метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 210
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_picture/
is_root: false
---
##  add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) Объект изображения.


```python
def add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| lower_right_row | int | Нижний индекс правой строки|
| lower_right_column | int | Индекс нижнего правого столбца|
| stream | io.RawIOBase | Потоковый объект, содержащий данные изображения.|

###  Примеры

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 0, 1, 0, fs)

```


##  add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Добавляет изображение в коллекцию.


###  Возвращает

[Picture](/cells/ru/python-net/aspose.cells.drawing/picture) Объект изображения.


```python
def add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| stream | io.RawIOBase | Потоковый объект, содержащий данные изображения.|
| width_scale | int | Масштаб ширины изображения в процентах.|
| height_scale | int | Масштаб высоты изображения в процентах.|

###  Примеры

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 1, fs, 50, 60)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

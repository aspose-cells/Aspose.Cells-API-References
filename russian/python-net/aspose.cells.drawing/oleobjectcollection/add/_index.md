---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.drawing/oleobjectcollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, height, width, image_data) {#int-int-int-int-bytes}
Добавляет OleObject в коллекцию.


###  Возвращает

[OleObject](/cells/ru/python-net/aspose.cells.drawing/oleobject) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, height, width, image_data):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| height | int | Высота oleObject в пикселях.|
| width | int | Ширина oleObject в пикселях.|
| image_data | bytes | Изображение объекта ole в виде массива байтов.|


##  add(upper_left_row, upper_left_column, height, width, image_data, linked_file) {#int-int-int-int-bytes-str}
Добавляет связанный объект OleObject в коллекцию.


###  Возвращает

[OleObject](/cells/ru/python-net/aspose.cells.drawing/oleobject) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, height, width, image_data, linked_file):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| height | int | Высота oleObject в пикселях.|
| width | int | Ширина oleObject в пикселях.|
| image_data | bytes | Изображение объекта ole в виде массива байтов.|
| linked_file | str |  |



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [OleObject](/cells/ru/python-net/aspose.cells.drawing/oleobject)
* класс [OleObjectCollection](/cells/ru/python-net/aspose.cells.drawing/oleobjectcollection)

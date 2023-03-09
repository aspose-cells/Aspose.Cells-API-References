---
title: add_shape метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 260
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---
##  add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}
Добавляет фигуру на лист.


###  Возвращает

Объект формы.


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/ru/python-net/aspose.cells.drawing/msodrawingtype) | Тип рисунка МСО.|
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение Shape от его левой строки в единицах пикселя.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение Shape от его левого столбца в пикселях.|
| height | int | Представляет высоту объекта Shape в пикселях.|
| width | int | Представляет ширину Shape в пикселях.|
###  Примечания

Тип не может быть Chart/Comment/Picture/OleObject/Polygon/DialogBox.
###  Примеры


```python
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

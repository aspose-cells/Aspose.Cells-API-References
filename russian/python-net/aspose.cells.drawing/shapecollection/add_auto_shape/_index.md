---
title: add_auto_shape метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
Добавляет автофигуру на лист.


###  Возвращает

Объект формы.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| type | [AutoShapeType](/cells/ru/python-net/aspose.cells.drawing/autoshapetype) | Автоматический тип формы.|
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
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

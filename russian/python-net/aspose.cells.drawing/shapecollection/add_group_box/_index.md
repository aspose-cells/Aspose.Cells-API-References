---
title: add_group_box метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 110
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_group_box/
is_root: false
---
##  add_group_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет GroupBox на лист.


###  Возвращает

Объект GroupBox.


```python
def add_group_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение GroupBox от его левой строки в пикселях.|
| upper_left_column | int |Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение GroupBox от его левого столбца в пикселях.|
| height | int | Представляет высоту GroupBox в пикселях.|
| width | int |Представляет ширину GroupBox в пикселях.|

###  Пример

```python

# add a group box
groupBox = shapes.add_group_box(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

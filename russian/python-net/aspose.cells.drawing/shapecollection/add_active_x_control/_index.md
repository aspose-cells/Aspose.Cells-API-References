---
title: add_active_x_control метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
Создает элемент управления Activex.


###  Возвращает




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | Тип элемента управления.|
| top_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение Shape от его левой строки в единицах пикселя.|
| left_column | int |Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение Shape от его левого столбца в пикселях.|
| width | int | Представляет ширину Shape в пикселях.|
| height | int | Представляет высоту объекта Shape в пикселях.|

###  Пример

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

---
title: add_arc метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_arc/
is_root: false
---
##  add_arc(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет ArcShape на рабочий лист.


###  Возвращает

Объект ArcShape.


```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение ArcShape от его левой строки в пикселях.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение ArcShape от его левого столбца в пикселях.|
| height | int | Представляет высоту ArcShape в пикселях.|
| width | int |Представляет ширину ArcShape в пикселях.|

###  Примеры

```python

# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

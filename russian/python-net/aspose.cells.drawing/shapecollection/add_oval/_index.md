---
title: add_oval метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 200
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет овал на рабочий лист.


###  Возвращает

Овальный объект.


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение овала от его левой строки в единицах пикселя.|
| upper_left_column | int |Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение овала от его левого столбца в единицах пикселя.|
| height | int | Представляет высоту овала в пикселях.|
| width | int | Представляет ширину овала в пикселях.|

###  Пример

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

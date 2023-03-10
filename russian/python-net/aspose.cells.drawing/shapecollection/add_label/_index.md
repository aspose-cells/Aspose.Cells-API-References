---
title: add_label метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 130
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---
##  add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет метку на рабочий лист.


###  Возвращает

Объект метки.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение Label от его левой строки в единицах пикселя.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение Label от его левого столбца в пикселях.|
| height | int | Представляет высоту метки в пикселях.|
| width | int | Представляет ширину Label в пикселях.|

###  Пример

```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

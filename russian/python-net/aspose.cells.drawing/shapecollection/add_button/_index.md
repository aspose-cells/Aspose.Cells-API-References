---
title: add_button метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_button/
is_root: false
---
##  add_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет кнопку на рабочий лист.


###  Возвращает

Объект Кнопка.


```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение Button от его левой строки в пикселях.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение Button от его левого столбца в пикселях.|
| height | int | Представляет высоту Button в пикселях.|
| width | int | Представляет ширину Button в пикселях.|

###  Пример

```python

# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

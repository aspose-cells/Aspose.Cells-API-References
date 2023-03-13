---
title: add_radio_button метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 230
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_radio_button/
is_root: false
---
##  add_radio_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет RadioButton на лист.


###  Возвращает

Объект RadioButton.


```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение RadioButton от его левой строки в пикселях.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение RadioButton от его левого столбца в пикселях.|
| height | int | Представляет высоту RadioButton в пикселях.|
| width | int | Представляет ширину RadioButton в пикселях.|

###  Пример

```python

# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

---
title: add_combo_box метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_combo_box/
is_root: false
---
##  add_combo_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет ComboBox на лист.


###  Возвращает

Объект ComboBox.


```python
def add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение ComboBox от его левой строки в пикселях.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение ComboBox от его левого столбца в пикселях.|
| height | int | Представляет высоту ComboBox в пикселях.|
| width | int | Представляет ширину ComboBox в пикселях.|

###  Пример

```python

# add a combo box
comboBox = shapes.add_combo_box(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

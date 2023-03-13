---
title: add_text_box метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 310
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет текстовое поле на лист.


###  Возвращает

Объект [TextBox](/cells/ru/python-net/aspose.cells.drawing/textbox).


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение текстового поля от его левой строки в пикселях.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение текстового поля от его левого столбца в пикселях.|
| height | int | Представляет высоту текстового поля в пикселях.|
| width | int | Представляет ширину текстового поля в пикселях.|

###  Пример

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
* класс [TextBox](/cells/ru/python-net/aspose.cells.drawing/textbox)

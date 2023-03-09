---
title: add_scroll_bar метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 250
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/
is_root: false
---
##  add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Добавляет полосу прокрутки на рабочий лист.


###  Возвращает

Объект полосы прокрутки.


```python
def add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение полосы прокрутки от ее левой строки в пикселях.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int | Представляет горизонтальное смещение полосы прокрутки от ее левого столбца в пикселях.|
| height | int | Представляет высоту полосы прокрутки в пикселях.|
| width | int | Представляет ширину полосы прокрутки в пикселях.|

###  Примеры

```python

# add a scroll bar
scrollBar = shapes.add_scroll_bar(1, 0, 1, 0, 100, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

---
title: set_outline_borders метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells/unionrange/set_outline_borders/
is_root: false
---
##  set_outline_borders(border_styles, border_colors) {#list-aspose.pydrawing.Color[]}
Устанавливает границы линии вокруг диапазона ячеек.



```python
def set_outline_borders(self, border_styles, border_colors):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| border_styles | list | Стили границ.|
| border_colors | aspose.pydrawing.Color[] | Цвета границ.|
###  Примечания

Длина как borderStyles, так и borderStyles должна быть равна 4.
Порядок borderStyles и borderStyles должен быть сверху, снизу, слева, справа.

##  set_outline_borders(border_style, border_color) {#CellBorderType-aspose.pydrawing.Color}
Устанавливает границы контура вокруг диапазона ячеек с одинаковым стилем и цветом границы.



```python
def set_outline_borders(self, border_style, border_color):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| border_style | [CellBorderType](/cells/ru/python-net/aspose.cells/cellbordertype) | Пограничный стиль.|
| border_color | aspose.pydrawing.Color | Цвет границы.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [UnionRange](/cells/ru/python-net/aspose.cells/unionrange)

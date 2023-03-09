---
title: set_two_color_gradient метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells.drawing/gradientfill/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
Задает для указанной заливки двухцветный градиент.
Применяется только для Excel 2007.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Один цвет градиента.|
| color2 | aspose.pydrawing.Color | Два градиентных цвета.|
| style | [GradientStyleType](/cells/ru/python-net/aspose.cells.drawing/gradientstyletype) | Градиентный стиль затенения.|
| variant | int |Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырех вариантов на вкладке "Градиент" в диалоговом окне "Эффекты заливки". Если стиль — GradientStyle.FromCenter, аргумент Variant может принимать значения только 1 или 2.|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
Задает для указанной заливки двухцветный градиент.
Применяется только для Excel 2007.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Один цвет градиента.|
| transparency1 | float | Степень прозрачности цвета1 в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный).|
| color2 | aspose.pydrawing.Color | Два градиентных цвета.|
| transparency2 | float | Степень прозрачности цвета2 в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный).|
| style | [GradientStyleType](/cells/ru/python-net/aspose.cells.drawing/gradientstyletype) | Градиентный стиль затенения.|
| variant | int |Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырех вариантов на вкладке "Градиент" в диалоговом окне "Эффекты заливки". Если стиль — GradientStyle.FromCenter, аргумент Variant может принимать значения только 1 или 2.|



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [GradientFill](/cells/ru/python-net/aspose.cells.drawing/gradientfill)

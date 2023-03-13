---
title: set_one_color_gradient метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.drawing/gradientfill/set_one_color_gradient/
is_root: false
---
##  set_one_color_gradient(color, degree, style, variant) {#aspose.pydrawing.Color-float-GradientStyleType-int}
Задает для указанной заливки одноцветный градиент.
Применяется только для Excel 2007.



```python
def set_one_color_gradient(self, color, degree, style, variant):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Один цвет градиента.|
| degree | float | Степень градиента. Может принимать значение от 0,0 (темный) до 1,0 (светлый).|
| style | [GradientStyleType](/cells/ru/python-net/aspose.cells.drawing/gradientstyletype) | Градиентный стиль затенения.|
| variant | int |Градиентный вариант. Может принимать значение от 1 до 4, соответствующее одному из четырех вариантов на вкладке «Градиент» в диалоговом окне «Эффекты заливки». Если стиль — GradientStyle.FromCenter, аргумент Variant может иметь значение только 1 или 2.|



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [GradientFill](/cells/ru/python-net/aspose.cells.drawing/gradientfill)

---
title: set_preset_color_gradient метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.drawing/lineformat/set_preset_color_gradient/
is_root: false
---
##  set_preset_color_gradient(preset_color, style, variant) {#GradientPresetType-GradientStyleType-int}
Устанавливает для указанной заливки градиент предустановленного цвета.
Применяется только для Excel 2007.



```python
def set_preset_color_gradient(self, preset_color, style, variant):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| preset_color | [GradientPresetType](/cells/ru/python-net/aspose.cells.drawing/gradientpresettype) | Предустановленный тип цвета|
| style | [GradientStyleType](/cells/ru/python-net/aspose.cells.drawing/gradientstyletype) | Градиентный стиль затенения.|
| variant | int |Градиентный вариант. Может принимать значение от 1 до 4, соответствующее одному из четырех вариантов на вкладке «Градиент» в диалоговом окне «Эффекты заливки». Если стиль — GradientStyle.FromCenter, аргумент Variant может иметь значение только 1 или 2.|



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [LineFormat](/cells/ru/python-net/aspose.cells.drawing/lineformat)

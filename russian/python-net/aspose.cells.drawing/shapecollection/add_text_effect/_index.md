---
title: add_text_effect метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 330
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_text_effect/
is_root: false
---
##  add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width) {#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int}
Вставляет объект WordArt.


###  Возвращает

Возвращает объект Shape, представляющий новый объект WordArt.


```python
def add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| effect | [MsoPresetTextEffect](/cells/ru/python-net/aspose.cells.drawing/msopresettexteffect) | Предустановленный тип текстового эффекта mso.|
| text | str | Текст WordArt.|
| font_name | str | Название шрифта.|
| size | int | Размер шрифта|
| font_bold | bool | Указывает, является ли шрифт полужирным.|
| font_italic | bool | Указывает, является ли шрифт курсивом.|
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение фигуры от ее левой строки в единицах пикселя.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int |Представляет горизонтальное смещение фигуры от ее левого столбца в пикселях.|
| height | int | Представляет высоту фигуры в пикселях.|
| width | int | Представляет ширину фигуры в пикселях.|

###  Примеры

```python
from aspose.cells.drawing import MsoPresetTextEffect

# add a WordArt
wordArt1 = shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT10, "WordArt", "arial", 18, False, False, 3, 0, 3, 0, 200, 50)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

---
title: add_word_art метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 350
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_word_art/
is_root: false
---
##  add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width) {#PresetWordArtStyle-str-int-int-int-int-int-int}
Добавляет предустановленные WordArt начиная с Excel 2007.s


###  Возвращает




```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| style | [PresetWordArtStyle](/cells/ru/python-net/aspose.cells.drawing/presetwordartstyle) | Предустановленный стиль WordArt.|
| text | str | Текст.|
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение фигуры от ее левой строки в единицах пикселя.|
| upper_left_column | int | Индекс левого верхнего столбца.|
| left | int |Представляет горизонтальное смещение фигуры от ее левого столбца в пикселях.|
| height | int | Представляет высоту фигуры в пикселях.|
| width | int | Представляет ширину фигуры в пикселях.|

###  Примеры

```python
from aspose.cells.drawing import PresetWordArtStyle

# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)

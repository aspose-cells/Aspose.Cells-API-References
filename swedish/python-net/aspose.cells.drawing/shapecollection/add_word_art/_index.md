---
title: add_word_art metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 350
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_word_art/
is_root: false
---
##  add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width) {#PresetWordArtStyle-str-int-int-int-int-int-int}
Lägger till förinställd WordArt sedan Excel 2007.s


###  Returnerar




```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| style | [PresetWordArtStyle](/cells/sv/python-net/aspose.cells.drawing/presetwordartstyle) |Den förinställda WordArt-stilen.|
| text | str | Texten.|
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av formen från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar formhöjden, i pixelenhet.|
| width | int | Representerar formens bredd i pixelenhet.|

###  Exempel

```python
from aspose.cells.drawing import PresetWordArtStyle

# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)

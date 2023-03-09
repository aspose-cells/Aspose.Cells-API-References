---
title: add_word_art yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 350
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_word_art/
is_root: false
---
##  add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width) {#PresetWordArtStyle-str-int-int-int-int-int-int}
Excel 2007.s'den bu yana hazır WordArt ekler


###  İadeler




```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| style | [PresetWordArtStyle](/cells/tr/python-net/aspose.cells.drawing/presetwordartstyle) |Önceden ayarlanmış WordArt Stili.|
| text | str | Metin.|
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Şeklin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int |Sol üst sütun dizini.|
| left | int | Şeklin sol sütunundan yatay uzaklığını piksel birimi cinsinden temsil eder.|
| height | int | Piksel birimi cinsinden şeklin yüksekliğini temsil eder.|
| width | int | Şeklin genişliğini piksel birimi cinsinden temsil eder.|

###  Örnek

```python
from aspose.cells.drawing import PresetWordArtStyle

# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

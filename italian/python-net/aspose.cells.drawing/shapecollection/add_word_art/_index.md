---
title: metodo add_word_art
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 350
url: /it/python-net/aspose.cells.drawing/shapecollection/add_word_art/
is_root: false
---
##  add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width) {#PresetWordArtStyle-str-int-int-int-int-int-int}
Aggiunge WordArt preimpostato da Excel 2007.s


###  ritorna




```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| style | [PresetWordArtStyle](/cells/it/python-net/aspose.cells.drawing/presetwordartstyle) |Lo stile WordArt predefinito.|
| text | str | Il testo.|
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale della forma dalla riga sinistra, in unità di pixel.|
| upper_left_column | int |Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale della forma dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza della forma, in unità di pixel.|
| width | int | Rappresenta la larghezza della forma, in unità di pixel.|

###  Esempio

```python
from aspose.cells.drawing import PresetWordArtStyle

# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

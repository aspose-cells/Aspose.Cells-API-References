---
title: metodo add_text_effect
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 330
url: /it/python-net/aspose.cells.drawing/shapecollection/add_text_effect/
is_root: false
---
##  add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width) {#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int}
Inserisce un oggetto WordArt.


###  ritorna

Restituisce un oggetto Shape che rappresenta il nuovo oggetto WordArt.


```python
def add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| effect | [MsoPresetTextEffect](/cells/it/python-net/aspose.cells.drawing/msopresettexteffect) | Il tipo di effetto di testo preimpostato mso.|
| text | str | Il testo WordArt.|
| font_name | str | Il nome del carattere.|
| size | int | La dimensione del carattere|
| font_bold | bool | Indica se il carattere è in grassetto.|
| font_italic | bool | Indica se il carattere è corsivo.|
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale della forma dalla riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int |Rappresenta l'offset orizzontale della forma dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza della forma, in unità di pixel.|
| width | int | Rappresenta la larghezza della forma, in unità di pixel.|

###  Esempi

```python
from aspose.cells.drawing import MsoPresetTextEffect

# add a WordArt
wordArt1 = shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT10, "WordArt", "arial", 18, False, False, 3, 0, 3, 0, 200, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

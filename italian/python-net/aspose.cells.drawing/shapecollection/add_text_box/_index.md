---
title: metodo add_text_box
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 310
url: /it/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge una casella di testo al foglio di lavoro.


###  ritorna

Un oggetto [TextBox](/cells/it/python-net/aspose.cells.drawing/textbox).


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale della casella di testo dalla sua riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale della casella di testo dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza della casella di testo, in unità di pixel.|
| width | int | Rappresenta la larghezza della casella di testo, in unità di pixel.|

###  Esempi

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
* classe [TextBox](/cells/it/python-net/aspose.cells.drawing/textbox)

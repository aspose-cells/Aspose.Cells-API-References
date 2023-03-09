---
title: metodo add_check_box
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge una casella di controllo al foglio di lavoro.


###  ritorna

Il nuovo indice dell'oggetto CheckBox.


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int |Rappresenta l'offset verticale della casella di controllo dalla sua riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale della casella di testo dalla colonna di sinistra, in unità di pixel.|
| height | int | Altezza della casella di testo, in unità di pixel.|
| width | int | Larghezza della casella di testo, in unità di pixel.|

###  Esempi

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

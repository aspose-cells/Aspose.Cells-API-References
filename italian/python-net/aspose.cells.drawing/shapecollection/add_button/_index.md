---
title: metodo add_button
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 60
url: /it/python-net/aspose.cells.drawing/shapecollection/add_button/
is_root: false
---
##  add_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un pulsante al foglio di lavoro.


###  ritorna

Un oggetto Button.


```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di Button dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di Button dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di Button, in unità di pixel.|
| width | int | Rappresenta la larghezza di Button, in unità di pixel.|

###  Esempi

```python

# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

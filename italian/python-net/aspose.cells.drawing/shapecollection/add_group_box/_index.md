---
title: metodo add_group_box
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 110
url: /it/python-net/aspose.cells.drawing/shapecollection/add_group_box/
is_root: false
---
##  add_group_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un GroupBox al foglio di lavoro.


###  ritorna

Un oggetto GroupBox.


```python
def add_group_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di GroupBox dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di GroupBox dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di GroupBox, in unità di pixel.|
| width | int | Rappresenta la larghezza di GroupBox, in unità di pixel.|

###  Esempi

```python

# add a group box
groupBox = shapes.add_group_box(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

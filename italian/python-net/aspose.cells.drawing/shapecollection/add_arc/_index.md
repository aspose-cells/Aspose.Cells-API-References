---
title: metodo add_arc
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells.drawing/shapecollection/add_arc/
is_root: false
---
##  add_arc(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un ArcShape al foglio di lavoro.


###  ritorna

Un oggetto ArcShape.


```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di ArcShape dalla riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di ArcShape dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di ArcShape, in unità di pixel.|
| width | int |Rappresenta la larghezza di ArcShape, in unità di pixel.|

###  Esempio

```python

# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

---
title: metodo add_rectangle
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 240
url: /it/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un oggetto RectangleShape al foglio di lavoro.


###  ritorna

Oggetto RectangleShape.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di RectangleShape dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di RectangleShape dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di RectangleShape, in unità di pixel.|
| width | int | Rappresenta la larghezza di RectangleShape, in unità di pixel.|

###  Esempi

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

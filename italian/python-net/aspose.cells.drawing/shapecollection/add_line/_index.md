---
title: metodo add_line
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 150
url: /it/python-net/aspose.cells.drawing/shapecollection/add_line/
is_root: false
---
##  add_line(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un oggetto LineShape al foglio di lavoro.


###  ritorna

Un oggetto LineShape.


```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di LineShape dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int |Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di LineShape dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di LineShape, in unità di pixel.|
| width | int | Rappresenta la larghezza di LineShape, in unità di pixel.|

###  Esempio

```python

#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

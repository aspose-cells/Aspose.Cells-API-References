---
title: metodo add_oval
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 200
url: /it/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un ovale al foglio di lavoro.


###  ritorna

Un oggetto ovale.


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di Oval dalla riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di Oval dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di Oval, in unità di pixel.|
| width | int | Rappresenta la larghezza di Oval, in unità di pixel.|

###  Esempi

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

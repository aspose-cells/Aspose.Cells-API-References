---
title: metodo add_spinner
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 290
url: /it/python-net/aspose.cells.drawing/shapecollection/add_spinner/
is_root: false
---
##  add_spinner(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge uno Spinner al foglio di lavoro.


###  ritorna

Un oggetto Spinner.


```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int |Rappresenta l'offset verticale di Spinner dalla riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di Spinner dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di Spinner, in unità di pixel.|
| width | int | Rappresenta la larghezza di Spinner, in unità di pixel.|

###  Esempio

```python

# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

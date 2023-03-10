---
title: metodo add_scroll_bar
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 250
url: /it/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/
is_root: false
---
##  add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge una barra di scorrimento al foglio di lavoro.


###  ritorna

Oggetto ScrollBar.


```python
def add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di ScrollBar dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di ScrollBar dalla relativa colonna sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di ScrollBar, in unità di pixel.|
| width | int | Rappresenta la larghezza di ScrollBar, in unità di pixel.|

###  Esempio

```python

# add a scroll bar
scrollBar = shapes.add_scroll_bar(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

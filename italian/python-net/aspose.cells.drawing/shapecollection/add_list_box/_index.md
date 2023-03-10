---
title: metodo add_list_box
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 170
url: /it/python-net/aspose.cells.drawing/shapecollection/add_list_box/
is_root: false
---
##  add_list_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Aggiunge un ListBox al foglio di lavoro.


###  ritorna

Un oggetto ListBox.


```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale di ListBox dalla relativa riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale di ListBox dalla colonna di sinistra, in unità di pixel.|
| height | int | Rappresenta l'altezza di ListBox, in unità di pixel.|
| width | int | Rappresenta la larghezza di ListBox, in unità di pixel.|

###  Esempio

```python

# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

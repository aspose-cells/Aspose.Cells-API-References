---
title: metodo add_copy
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 90
url: /it/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
Aggiunge e copia una forma nel foglio di lavoro.


###  ritorna

Il nuovo indice dell'oggetto forma.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_shape | [Shape](/cells/it/python-net/aspose.cells.drawing/shape) | Forma sorgente.|
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale della casella di controllo dalla sua riga sinistra, in unità di pixel.|
| upper_left_column | int |Indice colonna in alto a sinistra.|
| left | int | Rappresenta l'offset orizzontale della casella di testo dalla colonna di sinistra, in unità di pixel.|

###  Esempio

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

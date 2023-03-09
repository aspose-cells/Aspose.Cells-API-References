---
title: metodo copy_in_range
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 380
url: /it/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
Copia le forme nell'intervallo nell'intervallo di destinazione.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection) | Forme di origine.|
| ca | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | L'intervallo di origine.|
| dest_row | int | L'indice della riga dest dell'intervallo dest.|
| dest_column | int | La colonna dest dell'intervallo dest.|
| is_contained | bool | Se copiare solo le forme contenute nell'intervallo.<br/> Se vero, copia solo le forme nell'intervallo.<br/> Altrimenti, funziona come MS Office.|

###  Esempi

```python
from aspose.cells import CellArea

# add a shape
shapes.add_rectangle(2, 0, 2, 0, 130, 130)
area2 = CellArea()
area2.start_column = 1
area2.start_row = 1
area2.end_column = 5
area2.end_row = 11
# copy
shapes.copy_in_range(shapes, area2, 12, 1, False)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

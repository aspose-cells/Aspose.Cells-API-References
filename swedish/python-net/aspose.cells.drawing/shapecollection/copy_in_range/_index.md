---
title: copy_in_range metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 380
url: /sv/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
Kopiera former i intervallet till destinationsintervallet.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection) | Källformer.|
| ca | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) | Källomfånget.|
| dest_row | int | Dest radindex för målintervallet.|
| dest_column | int | Målkolumnen i målintervallet.|
| is_contained | bool | Om endast de former som finns i intervallet kopieras.<br/> Om sant, kopierar endast formerna i intervallet.<br/> Annars fungerar det som MS Office.|

###  Exempel

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



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)

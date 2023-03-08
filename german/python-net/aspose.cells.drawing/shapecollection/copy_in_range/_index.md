---
title: copy_in_range Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 380
url: /de/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
Formen im Bereich in den Zielbereich kopieren.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection) | Quellformen.|
| ca | [CellArea](/cells/de/python-net/aspose.cells/cellarea) | Der Quellbereich.|
| dest_row | int | Der Zielzeilenindex des Zielbereichs.|
| dest_column | int | Die Zielspalte des Zielbereichs.|
| is_contained | bool | Ob nur die Formen kopieren, die im Bereich enthalten sind.<br/> Bei „true“ werden nur die Shapes im Bereich kopiert.<br/> Ansonsten funktioniert es wie MS Office.|

###  Beispiel

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



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)

---
title: delete_in_range metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 400
url: /sv/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
Ta bort former i intervallet. Kommentarsformer kommer inte att tas bort.



```python
def delete_in_range(self, ca):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| ca | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) |Omfånget. Om formerna finns i intervallet kommer de att tas bort.|

###  Exempel

```python
from aspose.cells import CellArea

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
area3 = CellArea()
area3.start_column = 0
area3.start_row = 5
area3.end_column = 5
area3.end_row = 8
# del
shapes.delete_in_range(area3)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)

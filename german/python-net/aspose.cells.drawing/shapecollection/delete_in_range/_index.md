---
title: delete_in_range Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 400
url: /de/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
Formen im Bereich löschen.Kommentarformen werden nicht gelöscht.



```python
def delete_in_range(self, ca):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| ca | [CellArea](/cells/de/python-net/aspose.cells/cellarea) | Der Bereich. Wenn die Formen im Bereich enthalten sind, werden sie entfernt.|

###  Beispiel

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



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)

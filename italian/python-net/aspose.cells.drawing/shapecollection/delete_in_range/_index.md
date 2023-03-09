---
title: metodo delete_in_range
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 400
url: /it/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
Elimina le forme nell'intervallo. Le forme dei commenti non verranno eliminate.



```python
def delete_in_range(self, ca):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| ca | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | L'intervallo. Se le forme sono contenute nell'intervallo, verranno rimosse.|

###  Esempio

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



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)

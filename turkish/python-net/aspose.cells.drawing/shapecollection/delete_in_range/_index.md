---
title: delete_in_range yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 400
url: /tr/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
Aralıktaki şekilleri silin. Yorum şekilleri silinmeyecek.



```python
def delete_in_range(self, ca):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| ca | [CellArea](/cells/tr/python-net/aspose.cells/cellarea) |Aralık. Şekiller aralığın içindeyse, bunlar kaldırılacaktır.|

###  örnekler

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



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

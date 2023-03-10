---
title: طريقة delete_in_range
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 400
url: /ar/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
احذف الأشكال الموجودة في النطاق. لن يتم حذف أشكال التعليقات.



```python
def delete_in_range(self, ca):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| ca | [CellArea](/cells/ar/python-net/aspose.cells/cellarea) |النطاق: إذا كانت الأشكال موجودة في النطاق ، فسيتم إزالتها.|

###  مثال

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



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)

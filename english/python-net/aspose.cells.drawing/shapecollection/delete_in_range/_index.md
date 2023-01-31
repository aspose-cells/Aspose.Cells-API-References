---
title: delete_in_range method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 400
url: /python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---

## delete_in_range(ca) {#CellArea}

Delete shapes in the range.Comment shapes will not be deleted.



```python
def delete_in_range(self, ca):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ca | [CellArea](/cells/python-net/aspose.cells/cellarea) | The range.If the shapes are contained in the range, they will be removed. |
### Example 


```
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



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

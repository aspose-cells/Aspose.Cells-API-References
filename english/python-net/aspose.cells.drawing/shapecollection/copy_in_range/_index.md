---
title: copy_in_range method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 380
url: /python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---

## copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}

Copy shapes in the range to destination range.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection) | Source shapes. |
| ca | [CellArea](/cells/python-net/aspose.cells/cellarea) | The source range. |
| dest_row | int | The dest row index of the dest range. |
| dest_column | int | The dest column of the dest range. |
| is_contained | bool | Whether only copy the shapes which are contained in the range.<br/>If true,only copies the shapes in the range. <br/>Otherwise,it works as MS Office. |
### Example 


```
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



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

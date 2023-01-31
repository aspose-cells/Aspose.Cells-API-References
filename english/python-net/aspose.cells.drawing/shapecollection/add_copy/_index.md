---
title: add_copy method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---

## add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}

Adds and copy a shape to the worksheet.

### Returns 


The new shape object index.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| source_shape | [Shape](/cells/python-net/aspose.cells.drawing/shape) | Source shape. |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of checkbox from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
### Example 


```

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

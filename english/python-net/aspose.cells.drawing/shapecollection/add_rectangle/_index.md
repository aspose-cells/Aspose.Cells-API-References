---
title: add_rectangle method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 240
url: /python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---

## add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}

Adds a RectangleShape to the worksheet.

### Returns 


A RectangleShape object.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of RectangleShape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | int | Represents the height of RectangleShape, in unit of pixel. |
| width | int | Represents the width of RectangleShape, in unit of pixel. |
### Example 


```

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

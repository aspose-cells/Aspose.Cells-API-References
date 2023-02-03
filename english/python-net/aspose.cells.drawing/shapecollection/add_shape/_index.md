---
title: add_shape method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 260
url: /python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---

## add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}

Adds a Shape to the worksheet.


### Returns 


A Shape object.


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [MsoDrawingType](/cells/python-net/aspose.cells.drawing/msodrawingtype) | Mso drawing type. |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |
### Remarks

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### Example 


```python
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

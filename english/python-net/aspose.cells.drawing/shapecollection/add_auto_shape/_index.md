---
title: add_auto_shape method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---

## add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}

Adds a AutoShape to the worksheet.

### Returns 


A Shape object.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [AutoShapeType](/cells/python-net/aspose.cells.drawing/autoshapetype) | Auto shape type. |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |
### Remarks

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox


### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

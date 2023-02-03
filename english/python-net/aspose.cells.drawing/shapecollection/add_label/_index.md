---
title: add_label method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 130
url: /python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---

## add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}

Adds a Label to the worksheet.


### Returns 


A Label object.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Label from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | int | Represents the height of Label, in unit of pixel. |
| width | int | Represents the width of Label, in unit of pixel. |

### Example 


```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

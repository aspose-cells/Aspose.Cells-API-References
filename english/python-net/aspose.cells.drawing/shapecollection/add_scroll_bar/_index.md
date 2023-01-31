---
title: add_scroll_bar method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 250
url: /python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/
is_root: false
---

## add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}

Adds a ScrollBar to the worksheet.

### Returns 


A ScrollBar object.


```python
def add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of ScrollBar from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | int | Represents the height of ScrollBar, in unit of pixel. |
| width | int | Represents the width of ScrollBar, in unit of pixel. |
### Example 


```

# add a scroll bar
scrollBar = shapes.add_scroll_bar(1, 0, 1, 0, 100, 50)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

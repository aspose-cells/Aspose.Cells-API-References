---
title: top_in_shape property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1070
url: /python-net/aspose.cells.drawing/shape/top_in_shape/
is_root: false
---

## top_in_shape property


Represents the vertical offset of shape from the top border of the parent shape, 
in unit of 1/4000 of height of the parent shape.

### Remarks 


Only Applies when this shape in the group or chart.

### Example 


```python

if shape.top_in_shape == 8000:
    shape.top_in_shape = 4000

```
### Definition:
```python
@property
def top_in_shape(self):
    ...
@top_in_shape.setter
def top_in_shape(self, value):
    ...
```

### See Also
* module [aspose.cells.drawing](../../)
* class [Shape](/cells/python-net/aspose.cells.drawing/shape)

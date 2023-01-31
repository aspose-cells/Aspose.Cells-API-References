---
title: get_locked_property method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 110
url: /python-net/aspose.cells.drawing/scrollbar/get_locked_property/
is_root: false
---

## get_locked_property(type) {#ShapeLockType}

Gets the value of locked property.

### Returns 


Returns  the value of locked property.


```python
def get_locked_property(self, type):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [ShapeLockType](/cells/python-net/aspose.cells.drawing/shapelocktype) | The type of the shape locked property. |
### Example 


```
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1



```



### See Also
* module [aspose.cells.drawing](../../)
* class [ScrollBar](/cells/python-net/aspose.cells.drawing/scrollbar)

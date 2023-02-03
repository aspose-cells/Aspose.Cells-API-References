---
title: ungroup method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 450
url: /python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---

## ungroup(group) {#GroupShape}

Ungroups the shape items.



```python
def ungroup(self, group):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| group | [GroupShape](/cells/python-net/aspose.cells.drawing/groupshape) | The group shape. |
### Remarks

If the group shape is grouped by another group shape,nothing will be done.
### Example 


```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# group
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)
# ungroup
shapes.ungroup(groupShape)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

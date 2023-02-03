---
title: delete_shape method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 410
url: /python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---

## delete_shape(shape) {#Shape}

Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.



```python
def delete_shape(self, shape):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| shape | [Shape](/cells/python-net/aspose.cells.drawing/shape) |  |

### Example 


```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

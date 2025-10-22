##ungroup method
## ungroup(self, group) {#aspose.cells.drawing.GroupShape}
Ungroups the shape items.
```python
def ungroup(self, group):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| group | aspose.cells.drawing.GroupShape | The group shape. |
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
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)

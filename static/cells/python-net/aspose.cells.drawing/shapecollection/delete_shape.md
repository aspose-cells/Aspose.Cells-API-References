##delete_shape method
## delete_shape(self, shape) {#aspose.cells.drawing.Shape}
Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.
```python
def delete_shape(self, shape):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| shape | aspose.cells.drawing.Shape |  |
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
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)

##top_in_shape property
## top_in_shape property
Represents the vertical offset of shape from the top border of the parent shape,
in unit of 1/4000 of height of the parent shape.
### Remarks
Only Applies when this shape in the group or chart.
### Example
```python
if shape.is_in_group and shape.top_in_shape == 8000:
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
* module [`aspose.cells.drawing`](../../)
* class [`OleObject`](/cells/python-net/aspose.cells.drawing/oleobject)

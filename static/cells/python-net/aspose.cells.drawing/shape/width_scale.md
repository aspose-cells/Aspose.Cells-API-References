##width_scale property
## width_scale property
Gets and sets the width scale, in unit of percent of the original picture width.
If the shape is not picture ,the WidthScale property only returns 100;
### Example
```python
if shape.width_scale == 3:
shape.width_scale = 1
```
### Definition:
```python
@property
def width_scale(self):
...
@width_scale.setter
def width_scale(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)

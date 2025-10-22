##x_angle property
## x_angle property
When the object is an angle marker, get or set the first angle in degrees.
### Remarks
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
### Definition:
```python
@property
def x_angle(self):
...
@x_angle.setter
def x_angle(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapePathPoint`](/cells/python-net/aspose.cells.drawing/shapepathpoint)

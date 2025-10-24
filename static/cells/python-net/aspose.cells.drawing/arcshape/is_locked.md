##is_locked property
## is_locked property
True means the object can not be modified when the sheet is protected.
Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.
### Example
```python
# Sets the specified shape to unlocked state
if shape.worksheet.is_protected and shape.is_locked:
shape.is_locked = False
# Sets the specified shape to a locked state
if shape.worksheet.is_protected and notshape.is_locked:
shape.is_locked = True
```
### Definition:
```python
@property
def is_locked(self):
...
@is_locked.setter
def is_locked(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ArcShape`](/cells/python-net/aspose.cells.drawing/arcshape)

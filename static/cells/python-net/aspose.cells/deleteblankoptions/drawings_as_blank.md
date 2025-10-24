##drawings_as_blank property
## drawings_as_blank property
Whether drawing related objects such as picture, shape, chart... will be taken as blank.
Default value is true.
### Remarks
When setting this property as false,
all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.
### Definition:
```python
@property
def drawings_as_blank(self):
...
@drawings_as_blank.setter
def drawings_as_blank(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`DeleteBlankOptions`](/cells/python-net/aspose.cells/deleteblankoptions)

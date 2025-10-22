##image_source_full_name property
## image_source_full_name property
Gets or sets the path and name of the source file for the linked image.
### Remarks
The default value is an empty string.
If SourceFullName is not an empty string, the image is linked.
If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.
### Definition:
```python
@property
def image_source_full_name(self):
...
@image_source_full_name.setter
def image_source_full_name(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`OleObject`](/cells/python-net/aspose.cells.drawing/oleobject)

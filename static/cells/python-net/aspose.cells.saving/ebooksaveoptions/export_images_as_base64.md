##export_images_as_base64 property
## export_images_as_base64 property
Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.
### Remarks
When this property is set to true image data is exported directly on the
img elements and separate files are not created.
### Definition:
```python
@property
def export_images_as_base64(self):
...
@export_images_as_base64.setter
def export_images_as_base64(self, value):
...
```
### See Also
* module [`aspose.cells.saving`](../../)
* class [`EbookSaveOptions`](/cells/python-net/aspose.cells.saving/ebooksaveoptions)

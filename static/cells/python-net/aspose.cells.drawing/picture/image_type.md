##image_type property
## image_type property
Gets the image format of the picture.
### Example
```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
if pic1.image_type == ImageType.PNG:
pass
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
if pic2.image_type == ImageType.JPEG:
pass
```
### Definition:
```python
@property
def image_type(self):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ImageType`](/cells/python-net/aspose.cells.drawing/imagetype)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)

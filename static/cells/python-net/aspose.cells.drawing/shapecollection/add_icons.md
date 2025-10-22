##add_icons method
## add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
Adds svg image.
### Returns
```python
def add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int | The height of shape, in unit of pixel. |
| width | int | The width of shape, in unit of pixel. |
| image_byte_data | bytes | The image byte data. |
| compatible_image_data | bytes | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |
### Example
```python
from aspose import pycore
import bytearray
import int
# add icon
with open("icon.svg", "rb") as fs:
len = pycore.cast(int, utils.filesize(fs))
imageData = bytearray(len)
fs.readinto(imageData)
picture = shapes.add_icons(4, 0, 5, 0, -1, -1, imageData, None)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)

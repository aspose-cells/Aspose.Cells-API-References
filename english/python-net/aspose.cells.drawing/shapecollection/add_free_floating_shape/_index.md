---
title: add_free_floating_shape method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 100
url: /python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---

## add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}

Adds a free floating shape to the worksheet.Only applies for line/image shape.


### Returns 





```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [MsoDrawingType](/cells/python-net/aspose.cells.drawing/msodrawingtype) | The shape type. |
| top | int | Represents the vertical  offset of shape from the worksheet's top row, in unit of pixel. |
| left | int | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | int | Represents the height of LineShape, in unit of pixel. |
| width | int | Represents the width of LineShape, in unit of pixel. |
| image_data | bytes | The image data,only applies for the picture. |
| is_original_size | bool | Whether the shape use original size if the shape is image. |

### Example 


```python
from aspose.cells.drawing import MsoDrawingType
import aspose.pycore

# add a line
floatingShape_Line = shapes.add_free_floating_shape(MsoDrawingType.LINE, 100, 100, 100, 50, None, False)
# add a picture
imageData = None
with open("image.jpg", "rb") as fs:
    len = aspose.pycore.cast(System.Int32, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
floatingShape_Picture = shapes.add_free_floating_shape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, False)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

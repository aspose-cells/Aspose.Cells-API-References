---
title: طريقة add_ole_object
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 180
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_ole_object/
is_root: false
---
##  add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data) {#int-int-int-int-int-int-bytes}
يضيف OleObject.


###  عائدات




```python
def add_ole_object(self, upper_left_row, top, upper_left_column, left, height, width, image_data):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int |  |
| top | int |  |
| upper_left_column | int |  |
| left | int |  |
| height | int |  |
| width | int |  |
| image_data | bytes |  |

###  مثال

```python
from aspose import pycore

with open("image.jpg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    oleObject = shapes.add_ole_object(4, 0, 5, 0, 300, 500, imageData)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)

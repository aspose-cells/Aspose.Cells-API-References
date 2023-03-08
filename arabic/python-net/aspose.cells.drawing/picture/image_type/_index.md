---
title: image_type الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 580
url: /ar/python-net/aspose.cells.drawing/picture/image_type/
is_root: false
---
##  image_type الملكية

يحصل على تنسيق صورة الصورة.

###  مثال

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
###  تعريف:
```python
@property
def image_type(self):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ImageType](/cells/ar/python-net/aspose.cells.drawing/imagetype)
* فئة [Picture](/cells/ar/python-net/aspose.cells.drawing/picture)

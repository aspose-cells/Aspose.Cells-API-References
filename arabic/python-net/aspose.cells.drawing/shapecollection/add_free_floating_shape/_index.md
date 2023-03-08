---
title: طريقة add_free_floating_shape
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 100
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
يضيف شكلاً عائمًا حرًا إلى ورقة العمل. ينطبق فقط على شكل الخط / الصورة.


###  عائدات




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/ar/python-net/aspose.cells.drawing/msodrawingtype) | نوع الشكل.|
| top | int |يمثل الإزاحة الرأسية للشكل من الصف العلوي بورقة العمل ، بوحدة البكسل.|
| left | int | يمثل الإزاحة الأفقية للشكل من العمود الأيسر لورقة العمل ، بوحدة البكسل.|
| height | int | يمثل ارتفاع LineShape بوحدة البكسل.|
| width | int | يمثل عرض LineShape بوحدة البكسل.|
| image_data | bytes | بيانات الصورة تنطبق فقط على الصورة.|
| is_original_size | bool | ما إذا كان الشكل يستخدم الحجم الأصلي إذا كان الشكل صورة أم لا.|

###  مثال

```python
from aspose import pycore
from aspose.cells.drawing import MsoDrawingType

# add a line
floatingShape_Line = shapes.add_free_floating_shape(MsoDrawingType.LINE, 100, 100, 100, 50, None, False)
# add a picture
imageData = None
with open("image.jpg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
floatingShape_Picture = shapes.add_free_floating_shape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, False)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)

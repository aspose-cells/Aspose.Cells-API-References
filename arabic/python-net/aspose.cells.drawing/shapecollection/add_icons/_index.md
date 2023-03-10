---
title: طريقة add_icons
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 120
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_icons/
is_root: false
---
##  add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
يضيف صورة svg.


###  عائدات




```python
def add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية للشكل من صفه الأيسر ، بوحدة البكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int | الإزاحة الأفقية للشكل من عمودها الأيسر ، بوحدة البكسل.|
| height | int | ارتفاع الشكل بوحدة البكسل.|
| width | int | عرض الشكل بوحدة البكسل.|
| image_byte_data | bytes | بيانات بايت الصورة.|
| compatible_image_data | bytes |بيانات الصورة المحولة من svg لكي تكون متوافقة مع Excel 2016 أو الإصدارات الأقل.|

###  مثال

```python
from aspose import pycore

# add icon
with open("icon.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)

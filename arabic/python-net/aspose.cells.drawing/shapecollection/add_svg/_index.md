---
title: طريقة add_svg
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 300
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_svg/
is_root: false
---
##  add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
يضيف صورة svg.


###  عائدات




```python
def add_svg(self, upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data):
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
| svg_data | bytes | بيانات الصورة svg.|
| compatible_image_data | bytes |بيانات الصورة المحولة من svg لكي تكون متوافقة مع Excel 2016 أو الإصدارات الأقل.|

###  مثال

```python
from aspose import pycore

#  add a svg
with open("image.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)

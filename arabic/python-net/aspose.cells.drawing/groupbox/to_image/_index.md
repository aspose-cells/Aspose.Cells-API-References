---
title: طريقة to_image
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 210
url: /ar/python-net/aspose.cells.drawing/groupbox/to_image/
is_root: false
---
##  to_image(stream, image_type) {#io.RawIOBase-ImageType}
ينشئ صورة الشكل ويحفظها في دفق بالتنسيق المحدد.



```python
def to_image(self, stream, image_type):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | تيار الإخراج.|
| image_type | [ImageType](/cells/ar/python-net/aspose.cells.drawing/imagetype) | النوع المراد حفظ الصورة به.|
###  ملاحظات

التنسيقات التالية مدعومة:
.bmp ، .gif ، .jpg ، .jpeg ، .tiff ، .emf.
###  أمثلة

```python
from aspose.cells.drawing import ImageType
from io import BytesIO

imageStream = BytesIO()
shape.to_image(imageStream, ImageType.PNG)

```


##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
يحفظ الشكل في ملف.



```python
def to_image(self, image_file, options):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| image_file | str |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

###  أمثلة

```python
from aspose.cells.rendering import ImageOrPrintOptions

op = ImageOrPrintOptions()
shape.to_image("exmaple.png", op)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
يحفظ الشكل إلى تيار.



```python
def to_image(self, stream, options):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

###  أمثلة

```python
from aspose.cells.rendering import ImageOrPrintOptions
from io import BytesIO

imageStream = BytesIO()
op = ImageOrPrintOptions()
shape.to_image(imageStream, op)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [GroupBox](/cells/ar/python-net/aspose.cells.drawing/groupbox)

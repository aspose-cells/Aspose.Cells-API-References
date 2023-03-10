---
title: add_free_floating_shape yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 100
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
Çalışma sayfasına serbest kayan bir şekil ekler. Yalnızca çizgi/görüntü şekli için geçerlidir.


###  İadeler




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/tr/python-net/aspose.cells.drawing/msodrawingtype) | şekil tipi.|
| top | int | Şeklin çalışma sayfasının üst satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| left | int |Çalışma sayfasının sol sütunundaki şeklin piksel cinsinden yatay uzaklığını temsil eder.|
| height | int | Piksel birimi cinsinden LineShape yüksekliğini temsil eder.|
| width | int | Piksel birimi cinsinden LineShape genişliğini temsil eder.|
| image_data | bytes | Görüntü verileri, yalnızca resim için geçerlidir.|
| is_original_size | bool | Şekil resim ise, şeklin orijinal boyutu kullanıp kullanmadığı.|

###  Örnek

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



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

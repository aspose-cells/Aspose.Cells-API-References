---
title: add_icons yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 120
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_icons/
is_root: false
---
##  add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
svg görüntüsü ekler.


###  İadeler




```python
def add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Şeklin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int | Sol üst sütun dizini.|
| left | int | Şeklin sol sütunundan piksel birimi cinsinden yatay kayması.|
| height | int | Şeklin piksel cinsinden yüksekliği.|
| width | int | Şeklin piksel birimi cinsinden genişliği.|
| image_byte_data | bytes | Görüntü bayt verileri.|
| compatible_image_data | bytes |Excel 2016 veya daha düşük sürümlerle uyumlu olması için svg'den dönüştürülmüş görüntü verileri.|

###  örnekler

```python
from aspose import pycore

# add icon
with open("icon.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

---
title: add_svg yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 300
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_svg/
is_root: false
---
##  add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
svg görüntüsü ekler.


###  İadeler




```python
def add_svg(self, upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Şeklin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int |Sol üst sütun dizini.|
| left | int | Şeklin sol sütunundan piksel birimi cinsinden yatay kayması.|
| height | int | Şeklin piksel birimi cinsinden yüksekliği.|
| width | int | Şeklin piksel birimi cinsinden genişliği.|
| svg_data | bytes | svg görüntü verileri.|
| compatible_image_data | bytes | Excel 2016 veya daha düşük sürümlerle uyumlu olması için svg'den dönüştürülmüş görüntü verileri.|

###  Örnek

```python
from aspose import pycore

#  add a svg
with open("image.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

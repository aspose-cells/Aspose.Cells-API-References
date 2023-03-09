---
title: add_auto_shape yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
Çalışma sayfasına bir Otomatik Şekil ekler.


###  İadeler

Bir Şekil nesnesi.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [AutoShapeType](/cells/tr/python-net/aspose.cells.drawing/autoshapetype) | Otomatik şekil türü.|
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Shape öğesinin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int |Sol üst sütun dizini.|
| left | int | Shape'in sol sütunundan yatay uzaklığını piksel birimi cinsinden temsil eder.|
| height | int | Şeklin yüksekliğini piksel birimi cinsinden temsil eder.|
| width | int | Şeklin genişliğini piksel birimi cinsinden temsil eder.|
###  Notlar

Tür, Grafik/Yorum/Resim/OleObject/Polygon/DialogBox olamaz
###  Örnek


```python
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

---
title: add_shape yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 260
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---
##  add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}
Çalışma sayfasına bir Şekil ekler.


###  İadeler

Bir Şekil nesnesi.


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/tr/python-net/aspose.cells.drawing/msodrawingtype) | Mso çizim türü.|
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
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

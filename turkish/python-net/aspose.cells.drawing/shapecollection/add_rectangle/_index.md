---
title: add_rectangle yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 240
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir RectangleShape ekler.


###  İadeler

Bir RectangleShape nesnesi.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | RectangleShape öğesinin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int | Sol üst sütun dizini.|
| left | int | RectangleShape öğesinin sol sütunundan piksel birimi cinsinden yatay uzaklığını temsil eder.|
| height | int | Piksel birimi cinsinden RectangleShape yüksekliğini temsil eder.|
| width | int | Piksel birimi cinsinden RectangleShape genişliğini temsil eder.|

###  örnekler

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

---
title: add_group_box yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 110
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_group_box/
is_root: false
---
##  add_group_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir GroupBox ekler.


###  İadeler

Bir GroupBox nesnesi.


```python
def add_group_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | GroupBox öğesinin sol satırından piksel birimi cinsinden dikey uzaklığını temsil eder.|
| upper_left_column | int |Sol üst sütun dizini.|
| left | int | GroupBox öğesinin sol sütunundan piksel birimi cinsinden yatay uzaklığını temsil eder.|
| height | int | Piksel birimi cinsinden GroupBox yüksekliğini temsil eder.|
| width | int |Piksel birimi cinsinden GroupBox genişliğini temsil eder.|

###  Örnek

```python

# add a group box
groupBox = shapes.add_group_box(1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

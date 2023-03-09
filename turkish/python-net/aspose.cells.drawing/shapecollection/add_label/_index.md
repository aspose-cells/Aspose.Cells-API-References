---
title: add_label yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 130
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---
##  add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir Etiket ekler.


###  İadeler

Bir Etiket nesnesi.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Label öğesinin sol satırından piksel birimi cinsinden dikey uzaklığını temsil eder.|
| upper_left_column | int |Sol üst sütun dizini.|
| left | int | Label öğesinin sol sütunundan piksel birimi cinsinden yatay uzaklığını temsil eder.|
| height | int | Etiketin piksel birimi cinsinden yüksekliğini temsil eder.|
| width | int | Etiket genişliğini piksel birimi cinsinden temsil eder.|

###  Örnek

```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

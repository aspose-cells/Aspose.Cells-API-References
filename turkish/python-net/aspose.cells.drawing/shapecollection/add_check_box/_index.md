---
title: add_check_box yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 70
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir onay kutusu ekler.


###  İadeler

Yeni CheckBox nesne dizini.


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int |Piksel birimi cinsinden, onay kutusunun sol satırından dikey uzaklığını temsil eder.|
| upper_left_column | int | Sol üst sütun dizini.|
| left | int | Metin kutusunun sol sütunundan yatay uzaklığını piksel birimi cinsinden temsil eder.|
| height | int | Metin kutusunun piksel birimi cinsinden yüksekliği.|
| width | int | Metin kutusunun piksel birimi cinsinden genişliği.|

###  örnekler

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

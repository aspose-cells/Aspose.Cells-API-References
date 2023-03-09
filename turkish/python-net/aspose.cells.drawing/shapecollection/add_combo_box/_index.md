---
title: add_combo_box yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 80
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_combo_box/
is_root: false
---
##  add_combo_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir ComboBox ekler.


###  İadeler

Bir ComboBox nesnesi.


```python
def add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | ComboBox öğesinin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int | Sol üst sütun dizini.|
| left | int | ComboBox öğesinin sol sütunundan piksel birimi cinsinden yatay uzaklığını temsil eder.|
| height | int | Piksel birimi cinsinden ComboBox yüksekliğini temsil eder.|
| width | int | Piksel birimi cinsinden ComboBox genişliğini temsil eder.|

###  örnekler

```python

# add a combo box
comboBox = shapes.add_combo_box(1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

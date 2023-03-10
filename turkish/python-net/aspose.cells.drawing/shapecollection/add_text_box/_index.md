---
title: add_text_box yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 310
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir metin kutusu ekler.


###  İadeler

Bir [TextBox](/cells/tr/python-net/aspose.cells.drawing/textbox) nesnesi.


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Metin kutusunun sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| upper_left_column | int | Sol üst sütun dizini.|
| left | int | Metin kutusunun sol sütunundan yatay uzaklığını piksel birimi cinsinden temsil eder.|
| height | int | Metin kutusunun yüksekliğini piksel birimi cinsinden temsil eder.|
| width | int | Metin kutusunun genişliğini piksel birimi cinsinden temsil eder.|

###  Örnek

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)
* sınıf [TextBox](/cells/tr/python-net/aspose.cells.drawing/textbox)

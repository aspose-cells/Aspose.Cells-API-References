---
title: add_scroll_bar yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 250
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/
is_root: false
---
##  add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Çalışma sayfasına bir ScrollBar ekler.


###  İadeler

Bir ScrollBar nesnesi.


```python
def add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| top | int | Piksel birimi cinsinden, ScrollBar öğesinin sol satırından dikey uzaklığını temsil eder.|
| upper_left_column | int |Sol üst sütun dizini.|
| left | int | Piksel birimi cinsinden, ScrollBar öğesinin sol sütunundan yatay uzaklığını temsil eder.|
| height | int | Piksel birimi cinsinden ScrollBar'ın yüksekliğini temsil eder.|
| width | int | Piksel birimi cinsinden ScrollBar'ın genişliğini temsil eder.|

###  Örnek

```python

# add a scroll bar
scrollBar = shapes.add_scroll_bar(1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

---
title: add_copy yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 90
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
Çalışma sayfasına bir şekil ekler ve kopyalar.


###  İadeler

Yeni şekil nesne dizini.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| source_shape | [Shape](/cells/tr/python-net/aspose.cells.drawing/shape) | Kaynak şekli.|
| upper_left_row | int | Sol üst sıra dizini.|
| top | int |Piksel birimi cinsinden, onay kutusunun sol satırından dikey uzaklığını temsil eder.|
| upper_left_column | int | Sol üst sütun dizini.|
| left | int | Metin kutusunun sol sütunundan yatay uzaklığını piksel birimi cinsinden temsil eder.|

###  Örnek

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)

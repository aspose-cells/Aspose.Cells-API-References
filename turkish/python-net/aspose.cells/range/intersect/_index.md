---
title: intersect yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 110
url: /tr/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
İki aralığın dikdörtgen kesişimini temsil eden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi döndürür.


###  İadeler

[Range](/cells/tr/python-net/aspose.cells/range) nesnesini döndürür


```python
def intersect(self, range):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| range | [Range](/cells/tr/python-net/aspose.cells/range) | kesişen aralık.|
###  Notlar

İki aralık kesişmezse, null değerini döndürür.
###  Örnek


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A3:A10")
# Get intersected range of the two ranges.
intersectRange = range1.intersect(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)

---
title: auto_fill yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells/range/auto_fill/
is_root: false
---
##  auto_fill(target) {#Range}
Hedef aralığı otomatik olarak doldurun.



```python
def auto_fill(self, target):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| target | [Range](/cells/tr/python-net/aspose.cells/range) | hedef aralığı.|

###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
source = cells.create_range("A1:A2")
target = cells.create_range("A3:A10")
# fill 3,4,5....10 to the range A3:A10
source.auto_fill(target)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  auto_fill(target, auto_fill_type) {#Range-AutoFillType}
Hedef aralığı otomatik olarak doldurun.



```python
def auto_fill(self, target, auto_fill_type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| target | [Range](/cells/tr/python-net/aspose.cells/range) | Hedeflenen aralık.|
| auto_fill_type | [AutoFillType](/cells/tr/python-net/aspose.cells/autofilltype) | Otomatik doldurma türü.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)

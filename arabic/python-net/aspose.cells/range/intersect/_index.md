---
title: طريقة intersect
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 110
url: /ar/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
إرجاع عنصر [Range](/cells/ar/python-net/aspose.cells/range) يمثل التقاطع المستطيل لنطاقين.


###  عائدات

إرجاع عنصر [Range](/cells/ar/python-net/aspose.cells/range)


```python
def intersect(self, range):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| range | [Range](/cells/ar/python-net/aspose.cells/range) | النطاق المتقاطع.|
###  ملاحظات

إذا لم يتم تقاطع النطاقين ، يتم إرجاع قيمة خالية.
###  مثال


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



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Range](/cells/ar/python-net/aspose.cells/range)

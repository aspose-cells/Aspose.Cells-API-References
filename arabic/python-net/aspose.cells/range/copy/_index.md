---
title: طريقة copy
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
ينسخ البيانات (بما في ذلك الصيغ) والتنسيق ورسم الكائنات وما إلى ذلك من نطاق المصدر.



```python
def copy(self, range):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| range | [Range](/cells/ar/python-net/aspose.cells/range) | المصدر [Range](/cells/ar/python-net/aspose.cells/range) كائن.|

###  أمثلة

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  copy(range, options) {#Range-PasteOptions}
نسخ النطاق مع خيارات لصق خاصة.



```python
def copy(self, range, options):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| range | [Range](/cells/ar/python-net/aspose.cells/range) | نطاق المصدر.|
| options | [PasteOptions](/cells/ar/python-net/aspose.cells/pasteoptions) | خيارات لصق خاصة.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Range](/cells/ar/python-net/aspose.cells/range)

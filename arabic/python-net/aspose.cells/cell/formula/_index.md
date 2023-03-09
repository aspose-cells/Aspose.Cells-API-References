---
title: formula الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 460
url: /ar/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula الملكية

يحصل أو يحدد formula من [Cell](/cells/ar/python-net/aspose.cells/cell).

###  ملاحظات

 تبدأ سلسلة formula دائمًا بعلامة يساوي (=).
ويرجى دائمًا استخدام الفاصلة (،) كمحدد للمعلمات ، مثل "= SUM (A1، E1، H2)".

###  أمثلة

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  تعريف:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)

---
title: evaluated_page_count الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count الملكية

قم بتقييم إجمالي عدد الصفحات في ورقة العمل هذه

###  أمثلة

يُظهر الرمز التالي أسرع طريقة للحصول على عدد صفحات ورقة العمل.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```
###  تعريف:
```python
@property
def evaluated_page_count(self):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.rendering](../../)
* فئة [SheetPrintingPreview](/cells/ar/python-net/aspose.cells.rendering/sheetprintingpreview)

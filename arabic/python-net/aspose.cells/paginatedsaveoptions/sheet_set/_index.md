---
title: sheet_set الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 240
url: /ar/python-net/aspose.cells/paginatedsaveoptions/sheet_set/
is_root: false
---
##  sheet_set الملكية

الحصول على الأوراق أو تعيينها للعرض. الافتراضي هو كل الأوراق المرئية في المصنف: [SheetSet.visible](/cells/ar/python-net/aspose.cells.rendering/sheetset#visible).

###  مثال

الكود التالي يعرض الورقة النشطة فقط لقوات الدفاع الشعبي.

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering import SheetSet

workbook = Workbook("Book1.xlsx")
activeSheetIndex = workbook.worksheets.active_sheet_index
pdfSaveOptions = PdfSaveOptions()
# set active sheet index to sheet set.
pdfSaveOptions.sheet_set = SheetSet([activeSheetIndex])
workbook.save("output.pdf", pdfSaveOptions)

```
###  تعريف:
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PaginatedSaveOptions](/cells/ar/python-net/aspose.cells/paginatedsaveoptions)
* فئة [SheetSet](/cells/ar/python-net/aspose.cells.rendering/sheetset)

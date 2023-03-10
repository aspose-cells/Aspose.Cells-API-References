---
title: sheet_set mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 240
url: /tr/python-net/aspose.cells/paginatedsaveoptions/sheet_set/
is_root: false
---
##  sheet_set mülk

İşlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.visible](/cells/tr/python-net/aspose.cells.rendering/sheetset#visible).

###  Örnek

Aşağıdaki kod yalnızca aktif sayfayı pdf'ye dönüştürür.

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
###  Tanım:
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PaginatedSaveOptions](/cells/tr/python-net/aspose.cells/paginatedsaveoptions)
* sınıf [SheetSet](/cells/tr/python-net/aspose.cells.rendering/sheetset)

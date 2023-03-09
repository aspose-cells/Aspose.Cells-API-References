---
title: evaluated_page_count mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count mülk

Bu çalışma sayfasının toplam sayfa sayısını değerlendirin

###  Örnek

Aşağıdaki kod, bir çalışma sayfasının sayfa sayısını almanın en hızlı yolunu gösterir.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```
###  Tanım:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.rendering](../../)
* sınıf [SheetPrintingPreview](/cells/tr/python-net/aspose.cells.rendering/sheetprintingpreview)

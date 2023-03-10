---
title: evaluated_page_count mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count mülk

Bu çalışma kitabının toplam sayfa sayısını değerlendirin

###  Örnek

Aşağıdaki kod, bir çalışma kitabının sayfa sayısını almanın en hızlı yolunu gösterir.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```
###  Tanım:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.rendering](../../)
* sınıf [WorkbookPrintingPreview](/cells/tr/python-net/aspose.cells.rendering/workbookprintingpreview)

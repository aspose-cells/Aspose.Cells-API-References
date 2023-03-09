---
title: page_scale mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 90
url: /tr/python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---
##  page_scale mülk

Sayfanın hesaplanan sayfa ölçeğini alır.
[PageSetup.zoom](/cells/tr/python-net/aspose.cells/pagesetup#zoom) ayarlanmışsa ayarlanan ölçeği döndürür.

###  örnekler

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```
###  Tanım:
```python
@property
def page_scale(self):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.rendering](../../)
* sınıf [SheetRender](/cells/tr/python-net/aspose.cells.rendering/sheetrender)

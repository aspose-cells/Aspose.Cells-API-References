---
title: evaluated_page_count fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count fastighet

Utvärdera det totala antalet sidor i detta kalkylblad

###  Exempel

Följande kod visar det snabbaste sättet att få sidantal i ett kalkylblad.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```
###  Definition:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Se även
* modul [aspose.cells.rendering](../../)
* klass [SheetPrintingPreview](/cells/sv/python-net/aspose.cells.rendering/sheetprintingpreview)

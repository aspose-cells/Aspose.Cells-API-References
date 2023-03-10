---
title: evaluated_page_count fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count fastighet

Utvärdera det totala antalet sidor i denna arbetsbok

###  Exempel

Följande kod visar det snabbaste sättet att få sidantal i en arbetsbok.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```
###  Definition:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Se även
* modul [aspose.cells.rendering](../../)
* klass [WorkbookPrintingPreview](/cells/sv/python-net/aspose.cells.rendering/workbookprintingpreview)

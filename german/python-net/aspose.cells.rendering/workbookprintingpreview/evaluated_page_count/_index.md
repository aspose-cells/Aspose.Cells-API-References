---
title: evaluated_page_count Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count Eigentum

Bewerten Sie die Gesamtseitenzahl dieser Arbeitsmappe

###  Beispiel

Der folgende Code zeigt den schnellsten Weg, um die Seitenanzahl einer Arbeitsmappe zu ermitteln.

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

###  Siehe auch
* Modul [aspose.cells.rendering](../../)
* Klasse [WorkbookPrintingPreview](/cells/de/python-net/aspose.cells.rendering/workbookprintingpreview)

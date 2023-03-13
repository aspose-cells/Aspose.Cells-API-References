---
title: evaluated_page_count Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count Eigentum

Bewerten Sie die Gesamtseitenzahl dieses Arbeitsblatts

###  Beispiel

Der folgende Code zeigt den schnellsten Weg, um die Seitenzahl eines Arbeitsblatts zu erhalten.

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

###  Siehe auch
* Modul [aspose.cells.rendering](../../)
* Klasse [SheetPrintingPreview](/cells/de/python-net/aspose.cells.rendering/sheetprintingpreview)

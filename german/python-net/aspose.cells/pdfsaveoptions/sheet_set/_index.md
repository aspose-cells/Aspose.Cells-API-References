---
title: sheet_set Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 400
url: /de/python-net/aspose.cells/pdfsaveoptions/sheet_set/
is_root: false
---
##  sheet_set Eigentum

Ruft die zu rendernden Blätter ab oder legt sie fest. Standardmäßig sind alle sichtbaren Blätter in der Arbeitsmappe: [SheetSet.visible](/cells/de/python-net/aspose.cells.rendering/sheetset#visible).

###  Beispiele

Der folgende Code rendert nur aktive Blätter in PDF.

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
###  Definition:
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PdfSaveOptions](/cells/de/python-net/aspose.cells/pdfsaveoptions)
* Klasse [SheetSet](/cells/de/python-net/aspose.cells.rendering/sheetset)

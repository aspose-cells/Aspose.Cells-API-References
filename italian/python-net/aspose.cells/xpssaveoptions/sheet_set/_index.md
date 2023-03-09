---
title: sheet_set proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 240
url: /it/python-net/aspose.cells/xpssaveoptions/sheet_set/
is_root: false
---
##  sheet_set proprietà

Ottiene o imposta i fogli di cui eseguire il rendering. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [SheetSet.visible](/cells/it/python-net/aspose.cells.rendering/sheetset#visible).

###  Esempi

Il codice seguente esegue il rendering solo dei fogli attivi in pdf.

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
###  Definizione:
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [SheetSet](/cells/it/python-net/aspose.cells.rendering/sheetset)
* classe [XpsSaveOptions](/cells/it/python-net/aspose.cells/xpssaveoptions)

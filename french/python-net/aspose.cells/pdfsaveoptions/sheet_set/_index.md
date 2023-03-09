---
title: sheet_set propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 400
url: /fr/python-net/aspose.cells/pdfsaveoptions/sheet_set/
is_root: false
---
##  sheet_set propriété

Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles dans le classeur : [SheetSet.visible](/cells/fr/python-net/aspose.cells.rendering/sheetset#visible).

###  Exemple

Le code suivant rend uniquement la feuille active au format pdf.

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
###  Définition:
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [PdfSaveOptions](/cells/fr/python-net/aspose.cells/pdfsaveoptions)
* classe [SheetSet](/cells/fr/python-net/aspose.cells.rendering/sheetset)

---
title: sheet_set propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 400
url: /es/python-net/aspose.cells/pdfsaveoptions/sheet_set/
is_root: false
---
##  sheet_set propiedad

Obtiene o establece las hojas para representar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [SheetSet.visible](/cells/es/python-net/aspose.cells.rendering/sheetset#visible).

###  Ejemplo

El siguiente código solo convierte la hoja activa en pdf.

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
###  Definición:
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [PdfSaveOptions](/cells/es/python-net/aspose.cells/pdfsaveoptions)
* clase [SheetSet](/cells/es/python-net/aspose.cells.rendering/sheetset)

---
title: page_scale proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 90
url: /it/python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---
##  page_scale proprietà

Ottiene la scala di pagina calcolata del foglio.
Restituisce la scala impostata se è impostato [PageSetup.zoom](/cells/it/python-net/aspose.cells/pagesetup#zoom).

###  Esempi

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```
###  Definizione:
```python
@property
def page_scale(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells.rendering](../../)
* classe [SheetRender](/cells/it/python-net/aspose.cells.rendering/sheetrender)

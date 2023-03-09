---
title: evaluated_page_count propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count propiedad

Evalúe el recuento total de páginas de esta hoja de trabajo

###  Ejemplos

El siguiente código muestra la forma más rápida de obtener un recuento de páginas de una hoja de cálculo.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```
###  Definición:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Ver también
* módulo [aspose.cells.rendering](../../)
* clase [SheetPrintingPreview](/cells/es/python-net/aspose.cells.rendering/sheetprintingpreview)

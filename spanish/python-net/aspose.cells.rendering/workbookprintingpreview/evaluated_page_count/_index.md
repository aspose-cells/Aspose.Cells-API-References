---
title: evaluated_page_count propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count propiedad

Evaluar el recuento total de páginas de este libro de trabajo

###  Ejemplo

El siguiente código muestra la forma más rápida de obtener el recuento de páginas de un libro de trabajo.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```
###  Definición:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Ver también
* módulo [aspose.cells.rendering](../../)
* clase [WorkbookPrintingPreview](/cells/es/python-net/aspose.cells.rendering/workbookprintingpreview)

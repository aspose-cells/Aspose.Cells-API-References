---
title: page_index propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 190
url: /es/python-net/aspose.cells/paginatedsaveoptions/page_index/
is_root: false
---
##  page_index propiedad

Obtiene o establece el índice basado en 0 de la primera página que se va a guardar.

###  Observaciones

El valor predeterminado es 0.

###  Ejemplos

El siguiente ejemplo muestra cómo representar un rango de páginas (3 y 4) en un archivo de Excel Microsoft a PDF.

```python
from aspose.cells import PdfSaveOptions, Workbook

# Open an Excel file
wb = Workbook("Book1.xlsx")
options = PdfSaveOptions()
# Print only Page 3 and Page 4 in the output PDF
# Starting page index (0-based index)
options.page_index = 3
# Number of pages to be printed
options.page_count = 2
# Save the PDF file
wb.save("output.pdf", options)

```
###  Definición:
```python
@property
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [PaginatedSaveOptions](/cells/es/python-net/aspose.cells/paginatedsaveoptions)

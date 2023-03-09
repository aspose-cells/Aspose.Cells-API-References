---
title: page_count propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 310
url: /es/python-net/aspose.cells/pdfsaveoptions/page_count/
is_root: false
---
##  page_count propiedad

Obtiene o establece el número de páginas que se van a guardar.

###  Observaciones

El valor predeterminado es System.Int32.MaxValue, lo que significa que se representarán todas las páginas.

###  Ejemplo

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
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [PdfSaveOptions](/cells/es/python-net/aspose.cells/pdfsaveoptions)

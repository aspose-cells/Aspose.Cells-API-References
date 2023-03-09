---
title: printing_page_type propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 210
url: /es/python-net/aspose.cells/paginatedsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type propiedad

Indica qué páginas no se imprimirán.

###  Observaciones

Si el contenido de la hoja es escaso, habrá algunas páginas totalmente en blanco en el archivo pdf de salida.
Si no desea estas páginas en blanco, puede usar esta opción para omitirlas.

###  Ejemplos

El siguiente código omite páginas en blanco o páginas que solo contienen algún contenido de estilo como fondo de celda, bordes.

```python
from aspose.cells import PdfSaveOptions, PrintingPageType, Workbook

wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# ignore blank pages
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_BLANK
wb.save("output_ignore_blank_page.pdf", pdfSaveOptions)
# ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_STYLE
wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions)

```
###  Definición:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [PaginatedSaveOptions](/cells/es/python-net/aspose.cells/paginatedsaveoptions)
* clase [PrintingPageType](/cells/es/python-net/aspose.cells/printingpagetype)

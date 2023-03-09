---
title: printing_page_type proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 350
url: /it/python-net/aspose.cells/pdfsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type proprietà

Indica quali pagine non verranno stampate.

###  Osservazioni

Se il contenuto del foglio è scarso, ci saranno alcune pagine completamente vuote nel file pdf di output.
Se non desideri queste pagine vuote, puoi utilizzare questa opzione per ometterle.

###  Esempio

Il codice seguente omette le pagine vuote o le pagine che contengono solo alcuni contenuti di stile come lo sfondo delle celle, i bordi.

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
###  Definizione:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [PdfSaveOptions](/cells/it/python-net/aspose.cells/pdfsaveoptions)
* classe [PrintingPageType](/cells/it/python-net/aspose.cells/printingpagetype)

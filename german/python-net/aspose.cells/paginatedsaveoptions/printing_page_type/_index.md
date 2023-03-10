---
title: printing_page_type Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 210
url: /de/python-net/aspose.cells/paginatedsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type Eigentum

Gibt an, welche Seiten nicht gedruckt werden.

###  Bemerkungen

Wenn der Inhalt des Blatts spärlich ist, werden einige Seiten in der PDF-Ausgabedatei vollständig leer sein.
Wenn Sie diese leeren Seiten nicht möchten, können Sie sie mit dieser Option weglassen.

###  Beispiel

Der folgende Code lässt leere Seiten oder Seiten aus, die nur einige Stilinhalte wie Zellenhintergrund oder Rahmen enthalten.

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
###  Definition:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PaginatedSaveOptions](/cells/de/python-net/aspose.cells/paginatedsaveoptions)
* Klasse [PrintingPageType](/cells/de/python-net/aspose.cells/printingpagetype)

---
title: printing_page_type fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 210
url: /sv/python-net/aspose.cells/pptxsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type fastighet

Indikerar vilka sidor som inte kommer att skrivas ut.

###  Anmärkningar

Om innehållet i arket är sparsamt kommer det att finnas några sidor som är helt tomma i den utgående pdf-filen.
Om du inte vill ha dessa tomma sidor kan du använda det här alternativet för att utelämna dem.

###  Exempel

Följande kod utesluter tomma sidor eller sidor som bara innehåller en del stilinnehåll som cellbakgrund, ramar.

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

###  Se även
* modul [aspose.cells](../../)
* klass [PptxSaveOptions](/cells/sv/python-net/aspose.cells/pptxsaveoptions)
* klass [PrintingPageType](/cells/sv/python-net/aspose.cells/printingpagetype)

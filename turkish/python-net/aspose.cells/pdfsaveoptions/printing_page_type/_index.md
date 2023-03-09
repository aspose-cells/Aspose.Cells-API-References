---
title: printing_page_type mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 350
url: /tr/python-net/aspose.cells/pdfsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type mülk

Hangi sayfaların yazdırılmayacağını belirtir.

###  Notlar

Sayfadaki içerik seyrekse, çıktı pdf dosyasında bazı sayfalar tamamen boş olacaktır.
Bu boş sayfaları istemiyorsanız, onları atlamak için bu seçeneği kullanabilirsiniz.

###  örnekler

Aşağıdaki kod, boş sayfaları veya yalnızca hücre arka planı, kenarlıklar gibi bazı stil içeriği içeren sayfaları atlar.

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
###  Tanım:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PdfSaveOptions](/cells/tr/python-net/aspose.cells/pdfsaveoptions)
* sınıf [PrintingPageType](/cells/tr/python-net/aspose.cells/printingpagetype)

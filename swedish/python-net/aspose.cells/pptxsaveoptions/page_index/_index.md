---
title: page_index fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 190
url: /sv/python-net/aspose.cells/pptxsaveoptions/page_index/
is_root: false
---
##  page_index fastighet

Hämtar eller ställer in det 0-baserade indexet för den första sidan som ska sparas.

###  Anmärkningar

Standard är 0.

###  Exempel

Följande exempel visar hur man renderar en rad sidor (3 och 4) i en Microsoft Excel-fil till PDF.

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
###  Definition:
```python
@property
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [PptxSaveOptions](/cells/sv/python-net/aspose.cells/pptxsaveoptions)

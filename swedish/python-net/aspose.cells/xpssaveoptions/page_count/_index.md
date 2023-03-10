---
title: page_count fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 180
url: /sv/python-net/aspose.cells/xpssaveoptions/page_count/
is_root: false
---
##  page_count fastighet

Hämtar eller ställer in antalet sidor som ska sparas.

###  Anmärkningar

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas..

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
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [XpsSaveOptions](/cells/sv/python-net/aspose.cells/xpssaveoptions)

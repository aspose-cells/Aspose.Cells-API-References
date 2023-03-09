---
title: page_index Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 320
url: /de/python-net/aspose.cells/pdfsaveoptions/page_index/
is_root: false
---
##  page_index Eigentum

Ruft den 0-basierten Index der ersten zu speichernden Seite ab oder legt diesen fest.

###  Bemerkungen

Standard ist 0.

###  Beispiele

Das folgende Beispiel zeigt, wie ein Seitenbereich (3 und 4) in einer Microsoft-Excel-Datei in PDF gerendert wird.

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

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PdfSaveOptions](/cells/de/python-net/aspose.cells/pdfsaveoptions)

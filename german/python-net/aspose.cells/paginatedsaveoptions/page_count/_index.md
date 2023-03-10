---
title: page_count Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells/paginatedsaveoptions/page_count/
is_root: false
---
##  page_count Eigentum

Ruft die Anzahl der zu speichernden Seiten ab oder legt diese fest.

###  Bemerkungen

Standard ist System.Int32.MaxValue, was bedeutet, dass alle Seiten gerendert werden.

###  Beispiel

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
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PaginatedSaveOptions](/cells/de/python-net/aspose.cells/paginatedsaveoptions)

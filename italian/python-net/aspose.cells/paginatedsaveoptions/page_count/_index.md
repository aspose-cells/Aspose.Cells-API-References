---
title: page_count proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 180
url: /it/python-net/aspose.cells/paginatedsaveoptions/page_count/
is_root: false
---
##  page_count proprietà

Ottiene o imposta il numero di pagine da salvare.

###  Osservazioni

L'impostazione predefinita è System.Int32.MaxValue, il che significa che verrà eseguito il rendering di tutte le pagine.

###  Esempio

L'esempio seguente mostra come eseguire il rendering di un intervallo di pagine (3 e 4) in un file Excel Microsoft in PDF.

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
###  Definizione:
```python
@property
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [PaginatedSaveOptions](/cells/it/python-net/aspose.cells/paginatedsaveoptions)

---
title: page_index proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 190
url: /it/python-net/aspose.cells/xpssaveoptions/page_index/
is_root: false
---
##  page_index proprietà

Ottiene o imposta l'indice in base 0 della prima pagina da salvare.

###  Osservazioni

Il valore predefinito è 0.

###  Esempi

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
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [XpsSaveOptions](/cells/it/python-net/aspose.cells/xpssaveoptions)

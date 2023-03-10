---
title: evaluated_page_count proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count proprietà

Valuta il conteggio totale delle pagine di questo foglio di lavoro

###  Esempio

Il codice seguente mostra il modo più rapido per ottenere il conteggio delle pagine di un foglio di lavoro.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```
###  Definizione:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells.rendering](../../)
* classe [SheetPrintingPreview](/cells/it/python-net/aspose.cells.rendering/sheetprintingpreview)

---
title: metodo copy
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
Copia i dati (comprese le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine.



```python
def copy(self, range):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| range | [Range](/cells/it/python-net/aspose.cells/range) | Fonte [Range](/cells/it/python-net/aspose.cells/range) oggetto.|

###  Esempi

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  copy(range, options) {#Range-PasteOptions}
Copia dell'intervallo con opzioni speciali di incolla.



```python
def copy(self, range, options):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| range | [Range](/cells/it/python-net/aspose.cells/range) | L'intervallo di origine.|
| options | [PasteOptions](/cells/it/python-net/aspose.cells/pasteoptions) | Le opzioni speciali di incolla.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Range](/cells/it/python-net/aspose.cells/range)

---
title: metodo intersect
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 110
url: /it/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
Restituisce un oggetto [Range](/cells/it/python-net/aspose.cells/range) che rappresenta l'intersezione rettangolare di due intervalli.


###  ritorna

Restituisce un oggetto [Range](/cells/it/python-net/aspose.cells/range)


```python
def intersect(self, range):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| range | [Range](/cells/it/python-net/aspose.cells/range) | La gamma intersecante.|
###  Osservazioni

Se i due intervalli non sono intersecati, restituisce null.
###  Esempi


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A3:A10")
# Get intersected range of the two ranges.
intersectRange = range1.intersect(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Range](/cells/it/python-net/aspose.cells/range)

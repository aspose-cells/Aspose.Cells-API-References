---
title: formula proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 460
url: /it/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula proprietà

Ottiene o imposta formula di [Cell](/cells/it/python-net/aspose.cells/cell).

###  Osservazioni

 Una stringa formula inizia sempre con un segno uguale (=).
E per favore usa sempre la virgola (,) come delimitatore di parametri, come "=SUM(A1, E1, H2)".

###  Esempio

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  Definizione:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)

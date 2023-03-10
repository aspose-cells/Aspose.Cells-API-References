---
title: formula fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 460
url: /sv/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula fastighet

Hämtar eller ställer in ett formula av [Cell](/cells/sv/python-net/aspose.cells/cell).

###  Anmärkningar

 En formula-sträng börjar alltid med ett likhetstecken (=).
Och använd alltid kommatecken(,) som parametrar avgränsare, till exempel "=SUM(A1, E1, H2)".

###  Exempel

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  Definition:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)

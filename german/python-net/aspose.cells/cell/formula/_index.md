---
title: formula Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 460
url: /de/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula Eigentum

Ruft eine formula der [Cell](/cells/de/python-net/aspose.cells/cell) ab oder legt sie fest.

###  Bemerkungen

 Ein formula-String beginnt immer mit einem Gleichheitszeichen (=).
Und verwenden Sie bitte immer Komma (,) als Parametertrennzeichen, z. B. "= SUMME (A1, E1, H2)".

###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)

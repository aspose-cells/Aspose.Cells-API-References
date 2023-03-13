---
title: formula propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 460
url: /fr/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula propriété

Obtient ou définit un formula du [Cell](/cells/fr/python-net/aspose.cells/cell).

###  Remarques

 Une chaîne formula commence toujours par un signe égal (=).
Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, comme "=SUM(A1, E1, H2)".

###  Exemple

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  Définition:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)

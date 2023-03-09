---
title: formula propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 460
url: /es/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula propiedad

Obtiene o establece un formula del [Cell](/cells/es/python-net/aspose.cells/cell).

###  Observaciones

 Una cadena formula siempre comienza con un signo igual (=).
Y utilice siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

###  Ejemplo

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  Definición:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)

---
title: intersect método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 110
url: /es/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
Devuelve un objeto [Range](/cells/es/python-net/aspose.cells/range) que representa la intersección rectangular de dos rangos.


###  Devoluciones

Devuelve un objeto [Range](/cells/es/python-net/aspose.cells/range)


```python
def intersect(self, range):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| range | [Range](/cells/es/python-net/aspose.cells/range) | El rango de intersección.|
###  Observaciones

Si los dos rangos no se cruzan, devuelve nulo.
###  Ejemplos


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



###  Ver también
* módulo [aspose.cells](../../)
* clase [Range](/cells/es/python-net/aspose.cells/range)

---
title: metodo auto_fill
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells/range/auto_fill/
is_root: false
---
##  auto_fill(target) {#Range}
Riempiono automaticamente l'intervallo target.



```python
def auto_fill(self, target):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| target | [Range](/cells/it/python-net/aspose.cells/range) | la fascia di destinazione.|

###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
source = cells.create_range("A1:A2")
target = cells.create_range("A3:A10")
# fill 3,4,5....10 to the range A3:A10
source.auto_fill(target)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  auto_fill(target, auto_fill_type) {#Range-AutoFillType}
Riempiono automaticamente l'intervallo target.



```python
def auto_fill(self, target, auto_fill_type):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| target | [Range](/cells/it/python-net/aspose.cells/range) | La gamma mirata.|
| auto_fill_type | [AutoFillType](/cells/it/python-net/aspose.cells/autofilltype) | Il tipo di riempimento automatico.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Range](/cells/it/python-net/aspose.cells/range)

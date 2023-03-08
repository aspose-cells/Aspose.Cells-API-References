---
title: auto_fill Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells/range/auto_fill/
is_root: false
---
##  auto_fill(target) {#Range}
Füllen Sie den Zielbereich automatisch aus.



```python
def auto_fill(self, target):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| target | [Range](/cells/de/python-net/aspose.cells/range) | den Zielbereich.|

###  Beispiel

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
Füllen Sie den Zielbereich automatisch aus.



```python
def auto_fill(self, target, auto_fill_type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| target | [Range](/cells/de/python-net/aspose.cells/range) | Die Zielreichweite.|
| auto_fill_type | [AutoFillType](/cells/de/python-net/aspose.cells/autofilltype) | Der Autofill-Typ.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)

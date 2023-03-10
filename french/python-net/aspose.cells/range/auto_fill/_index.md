---
title: auto_fill méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/range/auto_fill/
is_root: false
---
##  auto_fill(target) {#Range}
Remplit automatiquement la plage cible.



```python
def auto_fill(self, target):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| target | [Range](/cells/fr/python-net/aspose.cells/range) | la plage cible.|

###  Exemple

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
Remplit automatiquement la plage cible.



```python
def auto_fill(self, target, auto_fill_type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| target | [Range](/cells/fr/python-net/aspose.cells/range) | La gamme ciblée.|
| auto_fill_type | [AutoFillType](/cells/fr/python-net/aspose.cells/autofilltype) | Le type de remplissage automatique.|



###  Voir également
* module [aspose.cells](../../)
* classe [Range](/cells/fr/python-net/aspose.cells/range)

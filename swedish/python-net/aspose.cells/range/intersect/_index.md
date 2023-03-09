---
title: intersect metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 110
url: /sv/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
Returnerar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt som representerar den rektangulära skärningspunkten mellan två intervall.


###  Returnerar

Returnerar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt


```python
def intersect(self, range):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| range | [Range](/cells/sv/python-net/aspose.cells/range) | Det korsande området.|
###  Anmärkningar

Om de två områdena inte skärs, returneras null.
###  Exempel


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



###  Se även
* modul [aspose.cells](../../)
* klass [Range](/cells/sv/python-net/aspose.cells/range)

---
title: copy metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
Kopierar data (inklusive formler), formatering, rita objekt etc. från ett källområde.



```python
def copy(self, range):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| range | [Range](/cells/sv/python-net/aspose.cells/range) | Källa [Range](/cells/sv/python-net/aspose.cells/range) objekt.|

###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  copy(range, options) {#Range-PasteOptions}
Kopiera intervallet med specialalternativ för klistra in.



```python
def copy(self, range, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| range | [Range](/cells/sv/python-net/aspose.cells/range) | Källomfånget.|
| options | [PasteOptions](/cells/sv/python-net/aspose.cells/pasteoptions) | Klistra specialalternativ.|



###  Se även
* modul [aspose.cells](../../)
* klass [Range](/cells/sv/python-net/aspose.cells/range)

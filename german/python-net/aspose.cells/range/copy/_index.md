---
title: copy Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich.



```python
def copy(self, range):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| range | [Range](/cells/de/python-net/aspose.cells/range) | Quelle [Range](/cells/de/python-net/aspose.cells/range) Objekt.|

###  Beispiele

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
Kopieren des Bereichs mit speziellen Optionen zum Einfügen.



```python
def copy(self, range, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| range | [Range](/cells/de/python-net/aspose.cells/range) | Der Quellbereich.|
| options | [PasteOptions](/cells/de/python-net/aspose.cells/pasteoptions) | Die speziellen Optionen zum Einfügen.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)

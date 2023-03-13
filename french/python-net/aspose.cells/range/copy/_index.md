---
title: copy méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
Copie les données (y compris les formules), la mise en forme, les objets de dessin, etc. à partir d'une plage source.



```python
def copy(self, range):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| range | [Range](/cells/fr/python-net/aspose.cells/range) | Objet source [Range](/cells/fr/python-net/aspose.cells/range).|

###  Exemple

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
Copie de la plage avec des options spéciales de collage.



```python
def copy(self, range, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| range | [Range](/cells/fr/python-net/aspose.cells/range) | La plage source.|
| options | [PasteOptions](/cells/fr/python-net/aspose.cells/pasteoptions) | Les options spéciales de collage.|



###  Voir également
* module [aspose.cells](../../)
* classe [Range](/cells/fr/python-net/aspose.cells/range)

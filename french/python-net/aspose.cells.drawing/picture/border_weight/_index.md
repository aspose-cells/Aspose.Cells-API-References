---
title: border_weight propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 320
url: /fr/python-net/aspose.cells.drawing/picture/border_weight/
is_root: false
---
##  border_weight propriété

Obtient ou définit l'épaisseur de la bordure d'une image en unités de pt.

###  Exemple

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Set the border color of the picture
pic.border_line_color = Color.red
# Set the border width of the picture
pic.border_weight = 3
# Save the excel file.
workbook.save("result.xlsx")

```
###  Définition:
```python
@property
def border_weight(self):
    ...
@border_weight.setter
def border_weight(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Picture](/cells/fr/python-net/aspose.cells.drawing/picture)

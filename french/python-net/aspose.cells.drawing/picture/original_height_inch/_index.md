---
title: original_height_inch propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 940
url: /fr/python-net/aspose.cells.drawing/picture/original_height_inch/
is_root: false
---
##  original_height_inch propriété

Obtient la hauteur d'origine de l'image, en unités de pouces.

###  Exemples

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Gets the original height of the picture.
picHeightInch = pic.original_height_inch
# Save the excel file.
workbook.save("result.xlsx")

```
###  Définition:
```python
@property
def original_height_inch(self):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Picture](/cells/fr/python-net/aspose.cells.drawing/picture)

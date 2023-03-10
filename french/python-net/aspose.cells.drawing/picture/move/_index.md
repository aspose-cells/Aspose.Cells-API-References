---
title: move méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 150
url: /fr/python-net/aspose.cells.drawing/picture/move/
is_root: false
---
##  move(upper_left_row, upper_left_column) {#int-int}
Déplace l'image vers un emplacement spécifié.



```python
def move(self, upper_left_row, upper_left_column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| upper_left_column | int | Index de la colonne en haut à gauche.|

###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Set the new location of the picture
pic.move(2, 4)
# Save the excel file.
workbook.save("result.xlsx")

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Picture](/cells/fr/python-net/aspose.cells.drawing/picture)

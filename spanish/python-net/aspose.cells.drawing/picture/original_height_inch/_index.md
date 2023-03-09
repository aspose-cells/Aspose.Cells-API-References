---
title: original_height_inch propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 940
url: /es/python-net/aspose.cells.drawing/picture/original_height_inch/
is_root: false
---
##  original_height_inch propiedad

Obtiene la altura original de la imagen, en unidades de pulgadas.

###  Ejemplos

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
###  Definición:
```python
@property
def original_height_inch(self):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)

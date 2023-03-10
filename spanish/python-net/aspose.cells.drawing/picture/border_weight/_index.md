---
title: border_weight propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 320
url: /es/python-net/aspose.cells.drawing/picture/border_weight/
is_root: false
---
##  border_weight propiedad

Obtiene o establece el peso de la línea de borde de una imagen en unidades de pt.

###  Ejemplo

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
###  Definición:
```python
@property
def border_weight(self):
    ...
@border_weight.setter
def border_weight(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)

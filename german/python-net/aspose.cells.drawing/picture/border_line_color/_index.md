---
title: border_line_color Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 310
url: /de/python-net/aspose.cells.drawing/picture/border_line_color/
is_root: false
---
##  border_line_color Eigentum

Repräsentiert die Farbe der Rahmenlinie eines Bildes.

###  Beispiel

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
# Save the excel file.
workbook.save("result.xlsx")

```
###  Definition:
```python
@property
def border_line_color(self):
    ...
@border_line_color.setter
def border_line_color(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)

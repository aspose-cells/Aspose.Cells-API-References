---
title: original_height Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 920
url: /de/python-net/aspose.cells.drawing/picture/original_height/
is_root: false
---
##  original_height Eigentum

Ruft die ursprüngliche Höhe des Bildes ab.

###  Beispiel

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
picHeight = pic.original_height
# Save the excel file.
workbook.save("result.xlsx")

```
###  Definition:
```python
@property
def original_height(self):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)

---
title: original_width proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 950
url: /it/python-net/aspose.cells.drawing/picture/original_width/
is_root: false
---
##  original_width proprietà

Ottiene la larghezza originale dell'immagine.

###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Gets the original width of the picture.
picWidth = pic.original_width
# Save the excel file.
workbook.save("result.xlsx")

```
###  Definizione:
```python
@property
def original_width(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)

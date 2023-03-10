---
title: original_height_cm proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 930
url: /it/python-net/aspose.cells.drawing/picture/original_height_cm/
is_root: false
---
##  original_height_cm proprietà

Ottiene l'altezza originale dell'immagine, in unità di centimetri.

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
# Gets the original height of the picture.
picHeightCM = pic.original_height_cm
# Save the excel file.
workbook.save("result.xlsx")

```
###  Definizione:
```python
@property
def original_height_cm(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)

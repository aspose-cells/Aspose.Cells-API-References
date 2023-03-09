---
title: original_height fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 920
url: /sv/python-net/aspose.cells.drawing/picture/original_height/
is_root: false
---
##  original_height fastighet

Får bildens ursprungliga höjd.

###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](../../)
* klass [Picture](/cells/sv/python-net/aspose.cells.drawing/picture)

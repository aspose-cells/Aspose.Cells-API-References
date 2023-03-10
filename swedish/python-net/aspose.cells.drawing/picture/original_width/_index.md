---
title: original_width fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 950
url: /sv/python-net/aspose.cells.drawing/picture/original_width/
is_root: false
---
##  original_width fastighet

Får bildens ursprungliga bredd.

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
# Gets the original width of the picture.
picWidth = pic.original_width
# Save the excel file.
workbook.save("result.xlsx")

```
###  Definition:
```python
@property
def original_width(self):
    ...
```

###  Se även
* modul [aspose.cells.drawing](../../)
* klass [Picture](/cells/sv/python-net/aspose.cells.drawing/picture)

---
title: original_height_inch mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 940
url: /tr/python-net/aspose.cells.drawing/picture/original_height_inch/
is_root: false
---
##  original_height_inch mülk

Resmin orijinal yüksekliğini inç cinsinden alır.

###  örnekler

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
###  Tanım:
```python
@property
def original_height_inch(self):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)

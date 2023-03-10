---
title: border_weight mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 320
url: /tr/python-net/aspose.cells.drawing/picture/border_weight/
is_root: false
---
##  border_weight mülk

Bir resmin kenar çizgisinin ağırlığını pt birimi cinsinden alır veya ayarlar.

###  Örnek

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
###  Tanım:
```python
@property
def border_weight(self):
    ...
@border_weight.setter
def border_weight(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)

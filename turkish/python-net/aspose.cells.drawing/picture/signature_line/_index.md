---
title: signature_line mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1050
url: /tr/python-net/aspose.cells.drawing/picture/signature_line/
is_root: false
---
##  signature_line mülk

İmza satırını alır ve ayarlar

###  Örnek

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.
pic.signature_line = s
# Save the excel file.
workbook.save("result.xlsx")

```
###  Tanım:
```python
@property
def signature_line(self):
    ...
@signature_line.setter
def signature_line(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
* sınıf [SignatureLine](/cells/tr/python-net/aspose.cells.drawing/signatureline)

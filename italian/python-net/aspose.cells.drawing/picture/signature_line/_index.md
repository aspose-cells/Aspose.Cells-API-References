---
title: signature_line proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1050
url: /it/python-net/aspose.cells.drawing/picture/signature_line/
is_root: false
---
##  signature_line proprietà

Ottiene e imposta la riga della firma

###  Esempio

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
###  Definizione:
```python
@property
def signature_line(self):
    ...
@signature_line.setter
def signature_line(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)
* classe [SignatureLine](/cells/it/python-net/aspose.cells.drawing/signatureline)

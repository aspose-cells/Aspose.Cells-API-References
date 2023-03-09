---
title: signature_line propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1050
url: /fr/python-net/aspose.cells.drawing/picture/signature_line/
is_root: false
---
##  signature_line propriété

Obtient et définit la ligne de signature

###  Exemple

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
###  Définition:
```python
@property
def signature_line(self):
    ...
@signature_line.setter
def signature_line(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Picture](/cells/fr/python-net/aspose.cells.drawing/picture)
* classe [SignatureLine](/cells/fr/python-net/aspose.cells.drawing/signatureline)

---
title: SignatureLine clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 640
url: /es/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine clase
Representa la línea de la firma.



El tipo SignatureLine expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [SignatureLine()](/cells/es/python-net/aspose.cells.drawing/signatureline/__init__/#) | Construye una nueva instancia de SignatureLine|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [id](/cells/es/python-net/aspose.cells.drawing/signatureline/id) | Obtiene o establece el identificador de esta línea de firma.|
| [provider_id](/cells/es/python-net/aspose.cells.drawing/signatureline/provider_id) | Obtiene y establece la identificación del proveedor de la firma.|
| [signer](/cells/es/python-net/aspose.cells.drawing/signatureline/signer) | Obtiene y establece el firmante.|
| [title](/cells/es/python-net/aspose.cells.drawing/signatureline/title) | Obtiene y establece el título de cantante.|
| [email](/cells/es/python-net/aspose.cells.drawing/signatureline/email) | Obtiene y configura el correo electrónico del cantante.|
| [is_line](/cells/es/python-net/aspose.cells.drawing/signatureline/is_line) | Indica si se trata de una línea de firma.|
| [allow_comments](/cells/es/python-net/aspose.cells.drawing/signatureline/allow_comments) | Indica si se pueden adjuntar comentarios.|
| [show_signed_date](/cells/es/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Indica si muestra la fecha de firma.|
| [instructions](/cells/es/python-net/aspose.cells.drawing/signatureline/instructions) | Obtiene y establece el texto que se muestra al usuario en el momento de la firma.|



###  Ejemplos

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture
imgIndex = worksheet.pictures.add(1, 1, "sample.png")
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.SignatureLine property
pic.signature_line = s
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Ver también
* módulo [aspose.cells.drawing](..)

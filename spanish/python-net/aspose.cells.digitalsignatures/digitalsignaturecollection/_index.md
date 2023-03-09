---
title: DigitalSignatureCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  DigitalSignatureCollection clase
Proporciona una colección de firmas digitales adjuntas a un documento.



El tipo DigitalSignatureCollection expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [DigitalSignatureCollection()](/cells/es/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) |El constructor de DigitalSignatureCollection.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(digital_signature)](/cells/es/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) | Agregue una firma a la colección de firmas digitales.|



###  Ejemplos

El siguiente ejemplo muestra cómo validar firmas digitales.

```python
from aspose.cells import Workbook

# workbook from a signed source file
signedWorkbook = Workbook(r"signedFile.xlsx")
# wb.IsDigitallySigned is true when the workbook is signed already.
print(signedWorkbook.is_digitally_signed)
# get digitalSignature collection from workbook
existingDsc = signedWorkbook.get_digital_signature()
for existingDs in existingDsc:
    print(existingDs.comments)
    print(existingDs.sign_time)
    print(existingDs.is_valid)

```

###  Ver también
* módulo [aspose.cells.digitalsignatures](..)

---
title: DigitalSignatureCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  DigitalSignatureCollection klass
Tillhandahåller en samling digitala signaturer bifogade till ett dokument.



Typen DigitalSignatureCollection avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [DigitalSignatureCollection()](/cells/sv/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) |Konstruktören av DigitalSignatureCollection.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(digital_signature)](/cells/sv/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) | Lägg till en signatur till DigitalSignatureCollection.|



###  Exempel

Följande exempel visar hur man validerar digital signatur.

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

###  Se även
* modul [aspose.cells.digitalsignatures](..)

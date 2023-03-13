---
title: DigitalSignatureCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  DigitalSignatureCollection Klasse
Stellt eine Sammlung digitaler Signaturen bereit, die an ein Dokument angehängt sind.



Der Typ DigitalSignatureCollection macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [DigitalSignatureCollection()](/cells/de/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) |Der Konstruktor von DigitalSignatureCollection.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(digital_signature)](/cells/de/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) | Fügen Sie DigitalSignatureCollection eine Signatur hinzu.|



###  Beispiel

Das folgende Beispiel zeigt, wie die digitale Signatur validiert wird.

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

###  Siehe auch
* Modul [aspose.cells.digitalsignatures](..)

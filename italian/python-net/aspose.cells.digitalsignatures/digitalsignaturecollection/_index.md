---
title: classe DigitalSignatureCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  classe DigitalSignatureCollection
Fornisce una raccolta di firme digitali allegate a un documento.



Il tipo DigitalSignatureCollection espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [DigitalSignatureCollection()](/cells/it/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) | Il costruttore di DigitalSignatureCollection.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [add(digital_signature)](/cells/it/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) |Aggiungi una firma a DigitalSignatureCollection.|



###  Esempio

L'esempio seguente mostra come convalidare la firma digitale.

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

###  Guarda anche
* modulo [aspose.cells.digitalsignatures](..)

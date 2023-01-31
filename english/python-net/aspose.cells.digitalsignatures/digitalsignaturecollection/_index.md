---
title: DigitalSignatureCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---

## DigitalSignatureCollection class

Provides a collection of digital signatures attached to a document.



The DigitalSignatureCollection type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [DigitalSignatureCollection()](/cells/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) | The constructor of DigitalSignatureCollection. |


### Methods
| Method | Description |
| :- | :- |
| [add(digital_signature)](/cells/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) | Add one signature to DigitalSignatureCollection. |


### Example 


The following example shows how to validate digital signature.

```
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
### See Also

* module [aspose.cells.digitalsignatures](../)

##DigitalSignatureCollection class
## DigitalSignatureCollection class
Provides a collection of digital signatures attached to a document.
The DigitalSignatureCollection type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) | The constructor of DigitalSignatureCollection. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, digital_signature)`](/cells/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#aspose.cells.digitalsignatures.digitalsignature) | Add one signature to DigitalSignatureCollection. |
### Example
The following example shows how to validate digital signature.
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
### See Also
* module [`aspose.cells.digitalsignatures`](..)

##VbaProject class
## VbaProject class
Represents the VBA project.
The VbaProject type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [is_valid_signed](/cells/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | Indicates whether the signature of VBA project is valid or not. |
| [cert_raw_data](/cells/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Gets certificate raw data if this VBA project is signed. |
| [encoding](/cells/python-net/aspose.cells.vba/vbaproject/encoding) | Gets and sets the encoding of VBA project. |
| [name](/cells/python-net/aspose.cells.vba/vbaproject/name) | Gets and sets the name of the VBA project. |
| [is_signed](/cells/python-net/aspose.cells.vba/vbaproject/is_signed) | Indicates whether VBAcode is signed or not. |
| [is_protected](/cells/python-net/aspose.cells.vba/vbaproject/is_protected) | Indicates whether this VBA project is protected. |
| [islocked_for_viewing](/cells/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Indicates whether this VBA project is locked for viewing. |
| [modules](/cells/python-net/aspose.cells.vba/vbaproject/modules) | Gets all [`VbaModule`](/cells/python-net/aspose.cells.vba/vbamodule) objects. |
| [references](/cells/python-net/aspose.cells.vba/vbaproject/references) | Gets all references of VBA project. |
### Methods
| Method | Description |
| :- | :- |
| [`sign(self, digital_signature)`](/cells/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.digitalsignature) | Sign this VBA project by a DigitalSignature |
| [`protect(self, islocked_for_viewing, password)`](/cells/python-net/aspose.cells.vba/vbaproject/protect/#bool-system.string) | Protects or unprotects this VBA project. |
| [`copy(self, source)`](/cells/python-net/aspose.cells.vba/vbaproject/copy/#aspose.cells.vba.vbaproject) | Copy VBA project from other file. |
| [`validate_password(self, password)`](/cells/python-net/aspose.cells.vba/vbaproject/validate_password/#system.string) | Validates protection password. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells.vba`](..)
* class [`VbaModule`](/cells/python-net/aspose.cells.vba/vbamodule)

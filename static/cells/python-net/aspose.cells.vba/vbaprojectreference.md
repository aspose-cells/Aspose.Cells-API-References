##VbaProjectReference class
## VbaProjectReference class
Represents the reference of VBA project.
The VbaProjectReference type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [type](/cells/python-net/aspose.cells.vba/vbaprojectreference/type) | Gets the type of this reference. |
| [name](/cells/python-net/aspose.cells.vba/vbaprojectreference/name) | Gets and sets the name of the reference. |
| [libid](/cells/python-net/aspose.cells.vba/vbaprojectreference/libid) | Gets and sets the Libid of the reference. |
| [twiddledlibid](/cells/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | Gets and sets the twiddled Libid of the reference. |
| [extended_libid](/cells/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | Gets and sets the extended Libid of the reference. |
| [relative_libid](/cells/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) | Gets and sets the referenced VBA project's identifier with an relative path. |
### Methods
| Method | Description |
| :- | :- |
| [`copy(self, source)`](/cells/python-net/aspose.cells.vba/vbaprojectreference/copy/#aspose.cells.vba.vbaprojectreference) |  |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells.vba`](..)

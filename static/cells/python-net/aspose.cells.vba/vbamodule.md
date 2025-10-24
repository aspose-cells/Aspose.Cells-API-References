##VbaModule class
## VbaModule class
Represents the module in VBA project.
The VbaModule type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [name](/cells/python-net/aspose.cells.vba/vbamodule/name) | Gets and sets the name of Module. |
| [type](/cells/python-net/aspose.cells.vba/vbamodule/type) | Gets the type of module. |
| [binary_codes](/cells/python-net/aspose.cells.vba/vbamodule/binary_codes) | Gets and sets the binary codes of module. |
| [codes](/cells/python-net/aspose.cells.vba/vbamodule/codes) | Gets and sets the codes of module. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType
# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
index = vbaProject.modules.add(VbaModuleType.CLASS, "test")
#  Get vba module
vbaModule = vbaProject.modules[index]
#  Set codes
vbaModule.codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub"
# Saving the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells.vba`](..)

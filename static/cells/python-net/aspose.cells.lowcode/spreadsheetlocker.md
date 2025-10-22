##SpreadsheetLocker class
## SpreadsheetLocker class
Low code api to lock spreadsheet file.
The SpreadsheetLocker type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [`process(, template_file, result_file, open_password, write_password)`](/cells/python-net/aspose.cells.lowcode/spreadsheetlocker/process/#system.string-system.string-system.string-system.string) | Locks spreadsheet file with specified settings. |
| [`process(, load_options, save_options, open_password, write_password)`](/cells/python-net/aspose.cells.lowcode/spreadsheetlocker/process/#aspose.cells.lowcode.lowcodeloadoptions-aspose.cells.lowcode.lowcodesaveoptions-system.string-system.string) | Locks spreadsheet file with specified settings. |
| [`process(, load_options, save_options, open_password, write_password, workbook_password, workbook_type)`](/cells/python-net/aspose.cells.lowcode/spreadsheetlocker/process/#aspose.cells.lowcode.lowcodeloadoptions-aspose.cells.lowcode.lowcodesaveoptions-system.string-system.string-system.string-aspose.cells.protectiontype) | Locks spreadsheet file with specified settings. |
| [`process(, load_options, save_options, provider)`](/cells/python-net/aspose.cells.lowcode/spreadsheetlocker/process/#aspose.cells.lowcode.lowcodeloadoptions-aspose.cells.lowcode.lowcodesaveoptions-aspose.cells.lowcode.abstractlowcodeprotectionprovider) | Locks spreadsheet file with specified settings. |
### Example
```python
from aspose.cells.lowcode import SpreadsheetLocker
SpreadsheetLocker.process("template.xlsx", "locked.xlsx", "mypassword", "mypassword")
```
### See Also
* module [`aspose.cells.lowcode`](..)

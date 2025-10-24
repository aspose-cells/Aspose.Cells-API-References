##protect method
## protect(self, type) {#aspose.cells.ProtectionType}
Protects worksheet.
```python
def protect(self, type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.ProtectionType | Protection type. |
### Remarks
This method protects worksheet without password. It can protect worksheet in all versions of Excel file.
## protect(self, type, password, old_password) {#aspose.cells.ProtectionType-System.String-System.String}
Protects worksheet.
```python
def protect(self, type, password, old_password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.ProtectionType | Protection type. |
| password | System.String | Password. |
| old_password | System.String | If the worksheet is already protected by a password, please supply the old password.
### Remarks
This method can protect worksheet in all versions of Excel file.
### Example
```python
from aspose.cells import ProtectionType, Workbook
# Instantiating a Workbook object
excel = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = excel.worksheets[0]
# Protecting the worksheet with a password
worksheet.protect(ProtectionType.ALL, "aspose", None)
# Saving the modified Excel file in default (that is Excel 20003) format
excel.save("output.xls")
```
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)

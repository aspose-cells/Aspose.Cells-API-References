##calculate_on_open property
## calculate_on_open property
Indicates whether the application is required to perform a full calculation when the workbook is opened.
### Remarks
This property is only for saving the settings to resultant spreadsheet file
so that other applications(such as ms excel) may act accordingly when loading the resultant file.
For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically,
no matter what value has been set for this property.
### Definition:
```python
@property
def calculate_on_open(self):
...
@calculate_on_open.setter
def calculate_on_open(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FormulaSettings`](/cells/python-net/aspose.cells/formulasettings)

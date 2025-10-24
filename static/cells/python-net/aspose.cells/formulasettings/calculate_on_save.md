##calculate_on_save property
## calculate_on_save property
Indicates whether recalculate the workbook before saving the document, when in manual calculation mode.
### Remarks
This property is only for saving the settings to resultant spreadsheet file
so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file.
For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically,
no matter what value has been set for this property.
### Definition:
```python
@property
def calculate_on_save(self):
...
@calculate_on_save.setter
def calculate_on_save(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FormulaSettings`](/cells/python-net/aspose.cells/formulasettings)

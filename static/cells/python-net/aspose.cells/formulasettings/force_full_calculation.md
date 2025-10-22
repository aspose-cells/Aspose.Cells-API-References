##force_full_calculation property
## force_full_calculation property
Indicates whether calculates all formulas every time when a calculation is triggered.
### Remarks
This property is only for saving the settings to resultant spreadsheet file
so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file.
For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically,
no matter what value has been set for this property.
### Definition:
```python
@property
def force_full_calculation(self):
...
@force_full_calculation.setter
def force_full_calculation(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FormulaSettings`](/cells/python-net/aspose.cells/formulasettings)

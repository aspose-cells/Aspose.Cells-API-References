##calculation_mode property
## calculation_mode property
Gets or sets the mode for workbook calculation in ms excel.
### Remarks
This property is only for saving the settings to resultant spreadsheet file
so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file.
For performance consideration for most user's application, we do not calculate any formula in the workbook automatically,
no matter what mode has been set for this property.
If user needs to calculate formulas, please always call methods on different objects according to requirement:
[`Workbook.calculate_formula`](/cells/python-net/aspose.cells/workbook/calculate_formula), [`Worksheet.calculate_formula`](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[`Cell.calculate`](/cells/python-net/aspose.cells/cell/calculate), ...etc.
### Definition:
```python
@property
def calculation_mode(self):
...
@calculation_mode.setter
def calculation_mode(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CalcModeType`](/cells/python-net/aspose.cells/calcmodetype)
* class [`FormulaSettings`](/cells/python-net/aspose.cells/formulasettings)

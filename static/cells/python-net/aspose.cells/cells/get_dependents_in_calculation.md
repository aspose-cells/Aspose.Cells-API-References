##get_dependents_in_calculation method
## get_dependents_in_calculation(self, row, column, recursive) {#int-int-bool}
Gets all cells whose calculated result depends on specific cell.
### Returns
Enumerator to enumerate all dependents(Cell objects)
```python
def get_dependents_in_calculation(self, row, column, recursive):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | Row index of the specific cell |
| column | int | Column index of the specific cell. |
| recursive | bool | Whether returns those dependents which do not reference to the specific cell directly
### Remarks
To use this method, please make sure the workbook has been set with true value for
[`FormulaSettings.enable_calculation_chain`](/cells/python-net/aspose.cells/formulasettings#enable_calculation_chain) and has been fully calculated with this setting.
If there is no formula reference to this cell, null will be returned.
For more details and example, please see [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation)
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)

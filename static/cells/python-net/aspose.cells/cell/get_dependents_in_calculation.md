##get_dependents_in_calculation method
## get_dependents_in_calculation(self, recursive) {#bool}
Gets all cells whose calculated result depends on this cell.
### Returns
Enumerator to enumerate all dependents(Cell objects)
```python
def get_dependents_in_calculation(self, recursive):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| recursive | bool | Whether returns those dependents which do not reference to this cell directly
### Remarks
To use this method, please make sure the workbook has been set with true value for
[`FormulaSettings.enable_calculation_chain`](/cells/python-net/aspose.cells/formulasettings#enable_calculation_chain) and has been fully calculated with this setting.
If there is no formula reference to this cell, null will be returned.
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("B1").get_dependents_in_calculation(False)
print("B1's calculation dependents:")
for c in en:
print(c.name)
en = cells.get("B2").get_dependents_in_calculation(False)
print("B2's calculation dependents:")
for c in en:
print(c.name)
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)

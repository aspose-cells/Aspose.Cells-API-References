##get_precedents_in_calculation method
## get_precedents_in_calculation(self) {#}
Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.
### Returns
Enumerator to enumerate all references(ReferredArea)
```python
def get_precedents_in_calculation(self):
...
```
### Remarks
This method can only work with the situation that [`FormulaSettings.enable_calculation_chain`](/cells/python-net/aspose.cells/formulasettings#enable_calculation_chain)
is true for the workbook and the workbook has been fully calculated.
If this cell is not a formula or it does not reference to any other cells, null will be returned.
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("A2").get_precedents_in_calculation()
print("A2's calculation precedents:")
for r in en:
print(r)
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)

##get_dependents method
## get_dependents(self, is_all) {#bool}
Get all cells whose formula references to this cell directly.
```python
def get_dependents(self, is_all):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_all | bool | Indicates whether check formulas in other worksheets |
### Remarks
* If one reference containing this cell appears in one cell's formula, that cell will be taken as
the dependent of this cell, no matter the reference or this cell is used or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
this formula is still be taken as A2's dependent.
To get those formulas whose calculated results depend on this cell, please use [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation).When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked.
So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will
cause poor performance. For performance consideration, user should use [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation) instead.
Or, user may gather precedents map of all cells by [`Cell.get_precedents`](/cells/python-net/aspose.cells/cell/get_precedents) firstly,
and then build the dependents map according to the precedents map.
* If one reference containing this cell appears in one cell's formula, that cell will be taken as
the dependent of this cell, no matter the reference or this cell is used or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
this formula is still be taken as A2's dependent.
To get those formulas whose calculated results depend on this cell, please use [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation).When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked.
So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will
cause poor performance. For performance consideration, user should use [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation) instead.
Or, user may gather precedents map of all cells by [`Cell.get_precedents`](/cells/python-net/aspose.cells/cell/get_precedents) firstly,
and then build the dependents map according to the precedents map.
* If one reference containing this cell appears in one cell's formula, that cell will be taken as
the dependent of this cell, no matter the reference or this cell is used or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
this formula is still be taken as A2's dependent.
To get those formulas whose calculated results depend on this cell, please use [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation).When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked.
So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will
cause poor performance. For performance consideration, user should use [`Cell.get_dependents_in_calculation`](/cells/python-net/aspose.cells/cell/get_dependents_in_calculation) instead.
Or, user may gather precedents map of all cells by [`Cell.get_precedents`](/cells/python-net/aspose.cells/cell/get_precedents) firstly,
and then build the dependents map according to the precedents map.
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
print(dependents[i].name)
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)

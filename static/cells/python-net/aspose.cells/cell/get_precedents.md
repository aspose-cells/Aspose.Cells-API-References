##get_precedents method
## get_precedents(self) {#}
Gets all references appearing in this cell's formula.
### Returns
Collection of all references appearing in this cell's formula.
```python
def get_precedents(self):
...
```
### Remarks
* Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [`Cell.get_precedents_in_calculation`](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation).
* Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [`Cell.get_precedents_in_calculation`](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation).
* Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [`Cell.get_precedents_in_calculation`](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation).
### Example
```python
from aspose.cells import CellsHelper, Workbook
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1"
areas = cells.get("A1").get_precedents()
for i in range(len(areas)):
area = areas[i]
stringBuilder = []
if area.is_external_link:
stringBuilder.append("[")
stringBuilder.append(area.external_file_name)
stringBuilder.append("]")
stringBuilder.append(area.sheet_name)
stringBuilder.append("!")
stringBuilder.append(CellsHelper.cell_index_to_name(area.start_row, area.start_column))
if area.is_area:
stringBuilder.append(":")
stringBuilder.append(CellsHelper.cell_index_to_name(area.end_row, area.end_column))
print("".join(stringBuilder))
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`ReferredAreaCollection`](/cells/python-net/aspose.cells/referredareacollection)

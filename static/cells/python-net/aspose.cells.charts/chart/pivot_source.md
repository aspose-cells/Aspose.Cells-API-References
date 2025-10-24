##pivot_source property
## pivot_source property
The source is the data of the pivotTable.
If PivotSource is not empty ,the chart is PivotChart.
### Remarks
If the pivot table  "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls".
The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook.
If you set this property ,the previous data source setting will be lost.
### Definition:
```python
@property
def pivot_source(self):
...
@pivot_source.setter
def pivot_source(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`Chart`](/cells/python-net/aspose.cells.charts/chart)

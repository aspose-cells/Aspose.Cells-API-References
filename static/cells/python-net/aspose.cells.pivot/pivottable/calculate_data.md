##calculate_data method
## calculate_data(self) {#}
Calculates pivottable's data to cells.
```python
def calculate_data(self):
...
```
### Remarks
Cell.Value in the pivot range could not return the correct result if the method is not been called.
This method calculates data with an inner pivot cache,not original data source.
So if the data source is changed, please call RefreshData() method first.
## calculate_data(self, option) {#aspose.cells.pivot.PivotTableCalculateOption}
Calculating pivot tables with options
```python
def calculate_data(self, option):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| option | aspose.cells.pivot.PivotTableCalculateOption |  |
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotTable`](/cells/python-net/aspose.cells.pivot/pivottable)

##start_cell method
## start_cell(self, column_index) {#int}
Prepares to process a cell.
### Returns
whether this cell needs to be processed. false to ignore the cell and check the next one until reach the end of cells data of current row
```python
def start_cell(self, column_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| column_index | int | column index of the cell to be processed |
### Remarks
It will be called when reaching an existing cell in current row. Current row is the row of last call of [`LightCellsDataHandler.process_row`](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row).
### See Also
* module [`aspose.cells`](../../)
* class [`LightCellsDataHandler`](/cells/python-net/aspose.cells/lightcellsdatahandler)

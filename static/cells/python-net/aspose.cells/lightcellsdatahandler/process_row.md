##process_row method
## process_row(self, row) {#aspose.cells.Row}
Starts to process one row.
### Returns
whether this row's cells need to be processed. false to ignore all cells in this row.
```python
def process_row(self, row):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | aspose.cells.Row | Row object which is being processed currently. |
### Remarks
It will be called after row's properties such as height, style, ...etc. have been read. However, cells in this row has not been read yet.
### See Also
* module [`aspose.cells`](../../)
* class [`LightCellsDataHandler`](/cells/python-net/aspose.cells/lightcellsdatahandler)

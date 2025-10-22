##start_row method
## start_row(self, row_index) {#int}
Prepares to process a row.
### Returns
whether this row(properties or cells data) needs to be processed. false to ignore this row and its cells and check the next row.
```python
def start_row(self, row_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | the index of next row to be processed |
### See Also
* module [`aspose.cells`](../../)
* class [`LightCellsDataHandler`](/cells/python-net/aspose.cells/lightcellsdatahandler)

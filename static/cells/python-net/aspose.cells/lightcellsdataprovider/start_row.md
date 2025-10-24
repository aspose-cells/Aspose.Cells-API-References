##start_row method
## start_row(self, row) {#aspose.cells.Row}
Starts to save data of one row.
```python
def start_row(self, row):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | aspose.cells.Row | Row object for implementation to fill data. Its row index is the returned value of latest call of [`LightCellsDataProvider.next_row`](/cells/python-net/aspose.cells/lightcellsdataprovider/next_row).
### Remarks
It will be called at the beginning of saving a row and its cells data.
If current row has some custom properties such as height, style, ...etc.,
implementation should set those properties to given Row object here.
### See Also
* module [`aspose.cells`](../../)
* class [`LightCellsDataProvider`](/cells/python-net/aspose.cells/lightcellsdataprovider)

##next_row method
## next_row(self) {#}
Gets the next row to be saved.
### Returns
the next row index to be saved. -1 means the end of current sheet data has been reached and no further row of current sheet to be saved.
```python
def next_row(self):
...
```
### Remarks
It will be called at the beginning of saving a row and its cells data(before [`LightCellsDataProvider.start_row`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_row)).
### See Also
* module [`aspose.cells`](../../)
* class [`LightCellsDataProvider`](/cells/python-net/aspose.cells/lightcellsdataprovider)

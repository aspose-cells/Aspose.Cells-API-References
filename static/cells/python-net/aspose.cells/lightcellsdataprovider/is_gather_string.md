##is_gather_string method
## is_gather_string(self) {#}
Checks whether the current string value of cell needs to be gathered into a global pool.
### Returns
true if string value need to be gathered into a global pool for the resultant file.
```python
def is_gather_string(self):
...
```
### Remarks
Gathering string values will take advantage only when there are many duplicated string values for the cells provided by this implementation.
In this situation gathering string will save much memory and generate smaller resultant file.
If there are many string values for the cells provided by LightCellsDataProvider but few of them are same,
gathering string will cost more memory and time and has no advantage for the resultant file.
### See Also
* module [`aspose.cells`](../../)
* class [`LightCellsDataProvider`](/cells/python-net/aspose.cells/lightcellsdataprovider)

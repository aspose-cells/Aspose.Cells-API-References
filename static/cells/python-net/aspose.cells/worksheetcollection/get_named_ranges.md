##get_named_ranges method
## get_named_ranges(self) {#}
Gets all pre-defined named ranges in the spreadsheet.
### Returns
An array of Range objects.
If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name.
Returns null if the named range does not exist.
```python
def get_named_ranges(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`WorksheetCollection`](/cells/python-net/aspose.cells/worksheetcollection)

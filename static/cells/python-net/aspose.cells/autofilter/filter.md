##filter method
## filter(self, field_index, criteria) {#int-System.String}
Filters a list with specified criteria.
```python
def filter(self, field_index, criteria):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter
| criteria | System.String | The specified criteria (a string; for example, "101"). |
### Remarks
Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.
### See Also
* module [`aspose.cells`](../../)
* class [`AutoFilter`](/cells/python-net/aspose.cells/autofilter)

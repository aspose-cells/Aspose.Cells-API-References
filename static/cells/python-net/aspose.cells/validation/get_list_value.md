##get_list_value method
## get_list_value(self, row, column) {#int-int}
Get the value for list of the validation for the specified cell.
### Returns
The value to produce the list of this validation for the specified cell.
If the list references to a range, then the returned value will be a [`ReferredArea`](/cells/python-net/aspose.cells/referredarea) object;
Otherwise the returned value may be null, object[], or simple object.
```python
def get_list_value(self, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | The row index. |
| column | int | The column index. |
### Remarks
Only for validation whose type is List and has been applied to given cell,
otherwise null will be returned.
### See Also
* module [`aspose.cells`](../../)
* class [`ReferredArea`](/cells/python-net/aspose.cells/referredarea)
* class [`Validation`](/cells/python-net/aspose.cells/validation)

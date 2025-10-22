##delete_blank_rows method
## delete_blank_rows(self) {#}
Delete all blank rows which do not contain any data or other object.
```python
def delete_blank_rows(self):
...
```
## delete_blank_rows(self, options) {#aspose.cells.DeleteOptions}
Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table.
```python
def delete_blank_rows(self, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| options | aspose.cells.DeleteOptions | The options of deleting range. |
### Remarks
For blank rows that will be deleted, it is not only required that [`Row.is_blank`](/cells/python-net/aspose.cells/row#is_blank) should be true,
but also there should be no visible comment defined for any cell in those rows,
and no pivot table whose range intersects with them.
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)

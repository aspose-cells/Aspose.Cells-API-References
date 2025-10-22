##get_refers_to method
## get_refers_to(self, is_r1c1, is_local) {#bool-bool}
Get the reference of this Name.
```python
def get_refers_to(self, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the reference needs to be formatted as R1C1. |
| is_local | bool | Whether the reference needs to be formatted by locale. |
## get_refers_to(self, is_r1c1, is_local, row, column) {#bool-bool-int-int}
Get the reference of this Name based on specified cell.
```python
def get_refers_to(self, is_r1c1, is_local, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the reference needs to be formatted as R1C1. |
| is_local | bool | Whether the reference needs to be formatted by locale. |
| row | int | The row index of the cell. |
| column | int | The column index of the cell. |
### See Also
* module [`aspose.cells`](../../)
* class [`Name`](/cells/python-net/aspose.cells/name)

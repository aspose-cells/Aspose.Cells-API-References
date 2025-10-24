##get_formula2 method
## get_formula2(self, is_r1c1, is_local) {#bool-bool}
Gets the value or expression associated with this validation.
### Returns
The value or expression associated with this validation.
```python
def get_formula2(self, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
## get_formula2(self, is_r1c1, is_local, row, column) {#bool-bool-int-int}
Gets the value or expression associated with this validation for specific cell.
### Returns
The value or expression associated with this validation.
```python
def get_formula2(self, is_r1c1, is_local, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |
### See Also
* module [`aspose.cells`](../../)
* class [`Validation`](/cells/python-net/aspose.cells/validation)

##get_input_range method
## get_input_range(self, is_r1c1, is_local) {#bool-bool}
Gets the range used to fill the control.
### Returns
The range used to fill the control.
```python
def get_input_range(self, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
### Example
```python
range = shape.get_input_range(False, True)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)

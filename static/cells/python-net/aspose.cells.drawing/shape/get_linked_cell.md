##get_linked_cell method
## get_linked_cell(self, is_r1c1, is_local) {#bool-bool}
Gets the range linked to the control's value.
### Returns
The range linked to the control's value.
```python
def get_linked_cell(self, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
### Example
```python
# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)

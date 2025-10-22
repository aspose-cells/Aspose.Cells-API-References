##get_value method
## get_value {#int-int}
Gets cell value with given offset from the top-left of this area.
### Returns
"#REF!" if this area is invalid;
"#N/A" if given offset out of this area;
Otherwise return the cell value at given position.
```python
def get_value(self, row_offset, col_offset):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_offset | int | row offset from the start row of this area |
| col_offset | int | column offset from the start row of this area |
### See Also
* module [`aspose.cellsgridjs`](../../)
* class [`GridReferredArea`](/cells/python-net/aspose.cellsgridjs/gridreferredarea)

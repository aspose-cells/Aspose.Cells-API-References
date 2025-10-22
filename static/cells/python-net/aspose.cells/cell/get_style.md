##get_style method
## get_style(self) {#}
Gets the cell style.
### Returns
Style object.
```python
def get_style(self):
...
```
### Remarks
To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object.
This method is same with [`Cell.get_style`](/cells/python-net/aspose.cells/cell/get_style) with true value for the parameter.
## get_style(self, check_borders) {#bool}
If checkBorders is true, check whether other cells' borders will effect the style of this cell.
### Returns
Style object.
```python
def get_style(self, check_borders):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| check_borders | bool | Check other cells' borders |
### Remarks
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`Style`](/cells/python-net/aspose.cells/style)

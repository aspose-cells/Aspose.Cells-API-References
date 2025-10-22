##string_value property
## string_value property
Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself.
For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned.
The formatted cell value is same with what you can get from excel when copying a cell as text(such as
copying cell to text editor or exporting to csv).
### Definition:
```python
@property
def string_value(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)

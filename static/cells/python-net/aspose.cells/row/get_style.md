##get_style method
## get_style(self) {#}
Gets the style of this row.
```python
def get_style(self):
...
```
### Remarks
Modifying the returned style object directly takes no effect for this row or any cells in this row.
You have to call [`Row.apply_style`](/cells/python-net/aspose.cells/row/apply_style) or [`Row.set_style`](/cells/python-net/aspose.cells/row/set_style) method
to apply the change to this row.
Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings,
such as existing cells that have not been set style explicitly, or those that have not been instantiated)
### See Also
* module [`aspose.cells`](../../)
* class [`Row`](/cells/python-net/aspose.cells/row)
* class [`Style`](/cells/python-net/aspose.cells/style)

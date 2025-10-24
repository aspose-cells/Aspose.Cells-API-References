##get_style method
## get_style(self) {#}
Gets the style of this column.
```python
def get_style(self):
...
```
### Remarks
Modifying the returned style object directly takes no effect for this column or any cells in this column.
You have to call [`Column.apply_style`](/cells/python-net/aspose.cells/column/apply_style) or [`Column.set_style`](/cells/python-net/aspose.cells/column/set_style) method
to apply the change to this column.
Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings,
such as existing cells that have not been set style explicitly, or those that have not been instantiated)
### See Also
* module [`aspose.cells`](../../)
* class [`Column`](/cells/python-net/aspose.cells/column)
* class [`Style`](/cells/python-net/aspose.cells/style)

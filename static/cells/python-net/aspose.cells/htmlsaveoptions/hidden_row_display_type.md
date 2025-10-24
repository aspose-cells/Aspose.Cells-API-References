##hidden_row_display_type property
## hidden_row_display_type property
Hidden row(the height of this row is 0) in excel,before save this into html format,
if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output,
if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"
### Definition:
```python
@property
def hidden_row_display_type(self):
...
@hidden_row_display_type.setter
def hidden_row_display_type(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`HtmlHiddenRowDisplayType`](/cells/python-net/aspose.cells/htmlhiddenrowdisplaytype)
* class [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions)

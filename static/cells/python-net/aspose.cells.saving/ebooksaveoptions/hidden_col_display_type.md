##hidden_col_display_type property
## hidden_col_display_type property
Hidden column(the width of this column is 0) in excel,before save this into html format,
if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output,
if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"
### Definition:
```python
@property
def hidden_col_display_type(self):
...
@hidden_col_display_type.setter
def hidden_col_display_type(self, value):
...
```
### See Also
* module [`aspose.cells.saving`](../../)
* class [`EbookSaveOptions`](/cells/python-net/aspose.cells.saving/ebooksaveoptions)
* class [`HtmlHiddenColDisplayType`](/cells/python-net/aspose.cells/htmlhiddencoldisplaytype)

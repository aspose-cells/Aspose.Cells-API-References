##html_cross_string_type property
## html_cross_string_type property
Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.
By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel.
But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.
### Definition:
```python
@property
def html_cross_string_type(self):
...
@html_cross_string_type.setter
def html_cross_string_type(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`HtmlCrossType`](/cells/python-net/aspose.cells/htmlcrosstype)
* class [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions)

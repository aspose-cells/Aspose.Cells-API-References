##is_h_scroll_bar_visible property
## is_h_scroll_bar_visible property
Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.
### Remarks
The default value is true.
### Example
The following code makes the horizontal scroll bar invisible for the spreadsheet.
```python
#  Hide the horizontal scroll bar of the Excel file.
settings.is_h_scroll_bar_visible = False
```
### Definition:
```python
@property
def is_h_scroll_bar_visible(self):
...
@is_h_scroll_bar_visible.setter
def is_h_scroll_bar_visible(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`WorkbookSettings`](/cells/python-net/aspose.cells/workbooksettings)

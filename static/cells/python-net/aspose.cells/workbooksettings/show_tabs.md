##show_tabs property
## show_tabs property
Get or sets a value whether the Workbook tabs are displayed.
### Remarks
The default value is true.
### Example
The following code hides the Sheet Tabs and Tab Scrolling Buttons for the spreadsheet.
```python
#  Hide the spreadsheet tabs.
workbook.settings.show_tabs = False
```
### Definition:
```python
@property
def show_tabs(self):
...
@show_tabs.setter
def show_tabs(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`WorkbookSettings`](/cells/python-net/aspose.cells/workbooksettings)

##check_workbook_default_font property
## check_workbook_default_font property
When characters in the Excel are Unicode and not be set with correct font in cell style,
They may appear as block in pdf,image.
Set this to true to try to use workbook's default font to show these characters first.
### Remarks
Default is true.
### Definition:
```python
@property
def check_workbook_default_font(self):
...
@check_workbook_default_font.setter
def check_workbook_default_font(self, value):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`ImageOrPrintOptions`](/cells/python-net/aspose.cells.rendering/imageorprintoptions)

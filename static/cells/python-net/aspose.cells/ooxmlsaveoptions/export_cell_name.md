##export_cell_name property
## export_cell_name property
Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file.
If the output file may be accessed by SQL Server DTS, this value must be true.
Setting the value to false will highly increase the performance and reduce the file size when creating large file.
Default value is true.
### Definition:
```python
@property
def export_cell_name(self):
...
@export_cell_name.setter
def export_cell_name(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`OoxmlSaveOptions`](/cells/python-net/aspose.cells/ooxmlsaveoptions)

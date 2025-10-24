##save_as_single_file property
## save_as_single_file property
Indicates whether save the html as single file.
The default value is false.
### Remarks
If there are multiple worksheets or other required resources such as pictures in the workbook,
commonly those worksheets and other resources need to be saved into separate files.
For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring.
If so, user may set this property as true.
### Definition:
```python
@property
def save_as_single_file(self):
...
@save_as_single_file.setter
def save_as_single_file(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions)

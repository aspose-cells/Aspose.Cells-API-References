##max_row_count property
## max_row_count property
The maximum count of rows to be imported for one sheet.
### Remarks
Those rows exceeding this limit will be ignored
or extended to next sheet according to [`TxtLoadOptions.extend_to_next_sheet`](/cells/python-net/aspose.cells/txtloadoptions#extend_to_next_sheet).
This count includes the header rows([`TxtLoadOptions.header_rows_count`](/cells/python-net/aspose.cells/txtloadoptions#header_rows_count)).
The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576.
If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### Definition:
```python
@property
def max_row_count(self):
...
@max_row_count.setter
def max_row_count(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`TxtLoadOptions`](/cells/python-net/aspose.cells/txtloadoptions)

##max_column_count property
## max_column_count property
The maximum count of columns to be imported for one sheet.
### Remarks
Those columns exceeding this limit will be ignored
or extended to next sheet according to [`TxtLoadOptions.extend_to_next_sheet`](/cells/python-net/aspose.cells/txtloadoptions#extend_to_next_sheet).
This count includes the header columns([`TxtLoadOptions.header_columns_count`](/cells/python-net/aspose.cells/txtloadoptions#header_columns_count)).
The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384.
If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.
### Definition:
```python
@property
def max_column_count(self):
...
@max_column_count.setter
def max_column_count(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`TxtLoadOptions`](/cells/python-net/aspose.cells/txtloadoptions)

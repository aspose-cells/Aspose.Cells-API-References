##check_mixed_value_type property
## check_mixed_value_type property
False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance.
True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type
And the value type are mixed, the DataColumn's type will be string.
### Definition:
```python
@property
def check_mixed_value_type(self):
...
@check_mixed_value_type.setter
def check_mixed_value_type(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`ExportTableOptions`](/cells/python-net/aspose.cells/exporttableoptions)

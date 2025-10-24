##skip_error_value property
## skip_error_value property
Indicates whether skip invalid value for the column.
For example,if the column type is decimal ,the value is greater than decimal.MaxValue
and this property is true,we will not throw exception again.
The default value is false.
### Definition:
```python
@property
def skip_error_value(self):
...
@skip_error_value.setter
def skip_error_value(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`ExportTableOptions`](/cells/python-net/aspose.cells/exporttableoptions)

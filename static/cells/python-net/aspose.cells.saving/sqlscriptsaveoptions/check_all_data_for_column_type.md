##check_all_data_for_column_type property
## check_all_data_for_column_type property
Check all data to find columns' data type.
### Remarks
The default value is false, we only check the first row for performance.
If this property is true and the columns contains mixed value type, the columns' type will be text.
### Definition:
```python
@property
def check_all_data_for_column_type(self):
...
@check_all_data_for_column_type.setter
def check_all_data_for_column_type(self, value):
...
```
### See Also
* module [`aspose.cells.saving`](../../)
* class [`SqlScriptSaveOptions`](/cells/python-net/aspose.cells.saving/sqlscriptsaveoptions)

##is_excel_2003_compatible property
## is_excel_2003_compatible property
Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable,
if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters,
it will be truncated. if false, a string will not have the aforementioned restriction.
The default value is true.
### Definition:
```python
@property
def is_excel_2003_compatible(self):
...
@is_excel_2003_compatible.setter
def is_excel_2003_compatible(self, value):
...
```
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotTable`](/cells/python-net/aspose.cells.pivot/pivottable)

##ignore_pivot_tables property
## ignore_pivot_tables property
Indicates whether saving pivot tables.
### Remarks
The pivot table feature of OpenOffice has fewer settings compared to Excel, so their results of pivot table have many differences.
Sometimes it's better to ingore these pivot tables when saving .ods file.
### Definition:
```python
@property
def ignore_pivot_tables(self):
...
@ignore_pivot_tables.setter
def ignore_pivot_tables(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`OdsSaveOptions`](/cells/python-net/aspose.cells/odssaveoptions)

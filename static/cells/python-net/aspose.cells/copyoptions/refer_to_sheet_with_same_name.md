##refer_to_sheet_with_same_name property
## refer_to_sheet_with_same_name property
In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one,
the copied formulas should refer to source workbook.
However, for some situations user may need the copied formulas refer to worksheets with the same name
in the same workbook, such as when those worksheets have been copied before this copy operation,
then this property should be kept as true.
### Remarks
The default value is true.
### Definition:
```python
@property
def refer_to_sheet_with_same_name(self):
...
@refer_to_sheet_with_same_name.setter
def refer_to_sheet_with_same_name(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CopyOptions`](/cells/python-net/aspose.cells/copyoptions)

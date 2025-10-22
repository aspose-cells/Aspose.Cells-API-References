##sheet_name property
## sheet_name property
Indicates which sheet this reference is in.
### Remarks
If it references to multiple worksheets,
the returned value is just like the range expression in the formula.
For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".
### Definition:
```python
@property
def sheet_name(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`ReferredArea`](/cells/python-net/aspose.cells/referredarea)

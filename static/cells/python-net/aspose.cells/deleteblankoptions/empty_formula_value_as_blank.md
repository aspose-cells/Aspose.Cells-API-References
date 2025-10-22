##empty_formula_value_as_blank property
## empty_formula_value_as_blank property
Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string.
Default value is false.
### Remarks
Generally user should make sure the formulas have been calculated before deleting operation with this property as true.
Otherwise all newly cretaed formulas by normal apis such as [`Cell.formula`](/cells/python-net/aspose.cells/cell#formula) will be taken as blank and may be deleted
because before calculation their calculated results are all null.
### Definition:
```python
@property
def empty_formula_value_as_blank(self):
...
@empty_formula_value_as_blank.setter
def empty_formula_value_as_blank(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`DeleteBlankOptions`](/cells/python-net/aspose.cells/deleteblankoptions)

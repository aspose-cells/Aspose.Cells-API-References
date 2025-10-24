##formula2 property
## formula2 property
Gets and sets the value or expression associated with conditional formatting.
### Remarks
Please add all areas before setting formula.
For setting formula for this condition, if the input value starts with '=', then it will be taken as formula.
Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### Definition:
```python
@property
def formula2(self):
...
@formula2.setter
def formula2(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FormatCondition`](/cells/python-net/aspose.cells/formatcondition)

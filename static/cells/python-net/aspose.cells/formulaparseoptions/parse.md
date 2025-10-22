##parse property
## parse property
Whether parse given formula. Default is true.
If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them
or parsed formula data is required by other operations such as calculating formulas.
### Definition:
```python
@property
def parse(self):
...
@parse.setter
def parse(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FormulaParseOptions`](/cells/python-net/aspose.cells/formulaparseoptions)

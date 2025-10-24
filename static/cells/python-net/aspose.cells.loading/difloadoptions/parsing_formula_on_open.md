##parsing_formula_on_open property
## parsing_formula_on_open property
Indicates whether parsing the formula when reading the file.
### Remarks
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file
because the formulas in the files are stored with a string formula.
### Definition:
```python
@property
def parsing_formula_on_open(self):
...
@parsing_formula_on_open.setter
def parsing_formula_on_open(self, value):
...
```
### See Also
* module [`aspose.cells.loading`](../../)
* class [`DifLoadOptions`](/cells/python-net/aspose.cells.loading/difloadoptions)

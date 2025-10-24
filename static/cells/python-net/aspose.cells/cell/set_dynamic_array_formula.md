##set_dynamic_array_formula method
## set_dynamic_array_formula(self, array_formula, options, calculate_value) {#System.String-aspose.cells.FormulaParseOptions-bool}
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
### Returns
the range that the formula should spill into.
```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | the formula expression |
| options | aspose.cells.FormulaParseOptions | options to parse formula.
| calculate_value | bool | whether calculate this dynamic array formula for those cells in the spilled range. |
### Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into.
If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!".
But for such kind of situation we still return the whole range that this formula should spill into.
## set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value) {#System.String-aspose.cells.FormulaParseOptions-list-bool-bool}
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
### Returns
the range that the formula should spill into.
```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | the formula expression |
| options | aspose.cells.FormulaParseOptions | options to parse formula.
| values | list | values(calculated results) for those cells with given dynamic array formula |
| calculate_range | bool | Whether calculate the spilled range for this dynamic array formula.
| calculate_value | bool | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null
### Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into.
If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!".
But for such kind of situation we still return the whole range that this formula should spill into.
## set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts) {#System.String-aspose.cells.FormulaParseOptions-list-bool-bool-aspose.cells.CalculationOptions}
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
### Returns
the range that the formula should spill into.
```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | the formula expression |
| options | aspose.cells.FormulaParseOptions | options to parse formula.
| values | list | values(calculated results) for those cells with given dynamic array formula |
| calculate_range | bool | Whether calculate the spilled range for this dynamic array formula.
| calculate_value | bool | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null
| copts | aspose.cells.CalculationOptions | The options for calculating formula.
### Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into.
If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!".
But for such kind of situation we still return the whole range that this formula should spill into.
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`CellArea`](/cells/python-net/aspose.cells/cellarea)

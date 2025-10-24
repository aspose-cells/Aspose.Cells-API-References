##calculate_formula method
## calculate_formula(self, formula) {#System.String}
Calculates a formula.
### Returns
Calculated formula result.
```python
def calculate_formula(self, formula):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| formula | System.String | Formula to be calculated. |
## calculate_formula(self, formula, opts) {#System.String-aspose.cells.CalculationOptions}
Calculates a formula expression directly.
### Returns
Calculated result of given formula.
The returned object may be of possible types of [`Cell.value`](/cells/python-net/aspose.cells/cell#value), or ReferredArea.
```python
def calculate_formula(self, formula, opts):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| formula | System.String | Formula to be calculated. |
| opts | aspose.cells.CalculationOptions | Options for calculating formula |
### Remarks
The formula will be calculated just like it has been set to cell A1.
And the formula will be taken as normal formula.
If you need the formula be calculated as an array formula and to get an array for the calculated result,
please use [`Worksheet.calculate_array_formula`](/cells/python-net/aspose.cells/worksheet/calculate_array_formula) instead.
## calculate_formula(self, options, recursive) {#aspose.cells.CalculationOptions-bool}
Calculates all formulas in this worksheet.
```python
def calculate_formula(self, options, recursive):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| options | aspose.cells.CalculationOptions | Options for calculation |
| recursive | bool | True means if the worksheet' cells depend on the cells of other worksheets,
## calculate_formula(self, formula, p_opts, c_opts, base_cell_row, base_cell_column, calculation_data) {#System.String-aspose.cells.FormulaParseOptions-aspose.cells.CalculationOptions-int-int-aspose.cells.CalculationData}
Calculates a formula expression directly.
### Returns
Calculated result of given formula.
The returned object may be of possible types of [`Cell.value`](/cells/python-net/aspose.cells/cell#value), or ReferredArea.
```python
def calculate_formula(self, formula, p_opts, c_opts, base_cell_row, base_cell_column, calculation_data):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| formula | System.String | Formula to be calculated. |
| p_opts | aspose.cells.FormulaParseOptions | Options for parsing formula. |
| c_opts | aspose.cells.CalculationOptions | Options for calculating formula. |
| base_cell_row | int | The row index of the base cell. |
| base_cell_column | int | The column index of the base cell. |
| calculation_data | aspose.cells.CalculationData | The calculation data. It is used for the situation
### Remarks
The formula will be calculated just like it has been set to the specified base cell.
And the formula will be taken as normal formula. If you need the formula be calculated as an array formula
and to get an array for the calculated result, please use
[`Worksheet.calculate_array_formula`](/cells/python-net/aspose.cells/worksheet/calculate_array_formula) instead.
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)

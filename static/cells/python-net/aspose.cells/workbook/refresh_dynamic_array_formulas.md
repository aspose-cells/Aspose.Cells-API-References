##refresh_dynamic_array_formulas method
## refresh_dynamic_array_formulas(self, calculate) {#bool}
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)
Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.
```python
def refresh_dynamic_array_formulas(self, calculate):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| calculate | bool | Whether calculates and updates cell values for those dynamic array formulas |
## refresh_dynamic_array_formulas(self, calculate, copts) {#bool-aspose.cells.CalculationOptions}
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)
```python
def refresh_dynamic_array_formulas(self, calculate, copts):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| calculate | bool | Whether calculates and updates cell values for those dynamic array formulas |
| copts | aspose.cells.CalculationOptions | The options for calculating formulas |
### Remarks
For performance consideration, we do not refresh all dynamic array formulas automatically
when the formula itself or the data it references to changed.
So user need to call this method manually after those operations which may influence dynamic array formulas,
such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc.
For most formulas with functions, calculating the spill range also needs to calculating the formula,
so in general true value for "calculate" flag is preferred.
If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...),
simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...),
and all formulas will be calculated later(such as by [`Workbook.calculate_formula`](/cells/python-net/aspose.cells/workbook/calculate_formula)),
then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)

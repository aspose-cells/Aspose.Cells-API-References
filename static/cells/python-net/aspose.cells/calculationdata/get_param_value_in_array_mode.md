##get_param_value_in_array_mode method
## get_param_value_in_array_mode(self, index, max_row_count, max_column_count) {#int-int-int}
Gets the value(s) of the parameter at given index.
If the parameter is some kind of expression that needs to be calculated,
then it will be calculated in array mode.
### Returns
An array which contains all items represented by the specified parameter.
```python
def get_param_value_in_array_mode(self, index, max_row_count, max_column_count):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The index of the parameter(0 based) |
| max_row_count | int | The row count limit for the returned array.
| max_column_count | int | The column count limit for the returned array.
### Remarks
For an expression that needs to be calculated, taking A:A+B:B as an example:
In value mode it will be calculated to a single value according to current cell base.
But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array.
And for such kind of situation, it is better to specify the limit for the row/column count
(such as according to [`Cells.max_data_row`](/cells/python-net/aspose.cells/cells#max_data_row) and [`Cells.max_data_column`](/cells/python-net/aspose.cells/cells#max_data_column)),
otherwise the returned large array may increase memory cost with large amount of useless data.
### See Also
* module [`aspose.cells`](../../)
* class [`CalculationData`](/cells/python-net/aspose.cells/calculationdata)

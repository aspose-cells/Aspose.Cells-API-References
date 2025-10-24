##get_param_value method
## get_param_value(self, index) {#int}
Gets the represented value object of the parameter at given index.
### Returns
The calculated value of the parameter.
```python
def get_param_value(self, index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The index of the parameter(0 based) |
### Remarks
For one parameter:
If it is plain value, then returns the plain value itself;
If it is reference, then returns ReferredArea object;
If it references to dataset(s) with multiple values, then returns array of objects;
If it is some kind of expression that needs to be calculated, then it will be calculated in value mode
and generally a single value will be returned according to current cell base. For example,
if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned.
However, if this parameter has been specified as array mode
(by [`Workbook.update_custom_function_definition`](/cells/python-net/aspose.cells/workbook/update_custom_function_definition)
or [`FormulaParseOptions.custom_function_definition`](/cells/python-net/aspose.cells/formulaparseoptions#custom_function_definition)),
then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....
### See Also
* module [`aspose.cells`](../../)
* class [`CalculationData`](/cells/python-net/aspose.cells/calculationdata)

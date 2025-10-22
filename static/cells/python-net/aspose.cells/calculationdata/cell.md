##cell property
## cell property
Gets the Cell object where the function is in.
### Remarks
When calculating a formula without setting it to a cell,
such as by [`Worksheet.calculate_formula`](/cells/python-net/aspose.cells/worksheet/calculate_formula),
the formula will be calculated just like it has been set to cell A1,
so both [`CalculationData.cell_row`](/cells/python-net/aspose.cells/calculationdata#cell_row) and [`CalculationData.cell_column`](/cells/python-net/aspose.cells/calculationdata#cell_column) are 0.
However, cell A1 in the worksheet may has not been instantiated.
So for such kind of situation this property will be null.
### Definition:
```python
@property
def cell(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CalculationData`](/cells/python-net/aspose.cells/calculationdata)
* class [`Cell`](/cells/python-net/aspose.cells/cell)

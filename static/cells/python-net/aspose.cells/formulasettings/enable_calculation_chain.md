##enable_calculation_chain property
## enable_calculation_chain property
Whether enable calculation chain for formulas. Default is false.
### Remarks
When there are lots of formulas in the workbook and user needs to calculate them repeatedly
with modifying only a small part of them, it may be helpful for performance to enable the calculation chain.
On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory,
and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas.
After changing this property from false to true, the calculation chain will be analyzed and built
at the time of first calculation for the workbook, so the required time for the first calculation
may be more than normal calculation without chain.
### Definition:
```python
@property
def enable_calculation_chain(self):
...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FormulaSettings`](/cells/python-net/aspose.cells/formulasettings)

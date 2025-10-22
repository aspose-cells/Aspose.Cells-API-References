##calculated_value property
## calculated_value property
Gets or sets the calculated value for this function.
### Remarks
User should set this property in his custom calculation engine for those functions the engine supports,
and the set value will be returned when getting this property later.
The set value may be of possible types of [`Cell.value`](/cells/python-net/aspose.cells/cell#value),
or array of such kind of values, or a Range, Name, ReferredArea.
Getting this property before setting value to it will make the function be calculated
by the default calculation engine of Aspose.Cells and then the calculated value will
be returned(generally it should be #NAME? for user-defined functions).
### Definition:
```python
@property
def calculated_value(self):
...
@calculated_value.setter
def calculated_value(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CalculationData`](/cells/python-net/aspose.cells/calculationdata)

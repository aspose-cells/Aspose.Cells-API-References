##calculated_value property
## calculated_value property
Gets/sets the calculated value for this function.
### Remarks
User should set this property in his custom calculation engine for those functions the engine supports,
and the set value will be returned when getting this property.
Getting this property before setting will make the function be calculated by the default calculation engine of Aspose.Cells and the calculated value will be returned.
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
* module [`aspose.cellsgridjs`](../../)
* class [`GridCalculationData`](/cells/python-net/aspose.cellsgridjs/gridcalculationdata)

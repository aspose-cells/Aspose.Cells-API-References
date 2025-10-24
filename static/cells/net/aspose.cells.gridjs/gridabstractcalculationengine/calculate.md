##GridAbstractCalculationEngine.Calculate
GridAbstractCalculationEngine method. Calculates one function with given data
## GridAbstractCalculationEngine.Calculate method
Calculates one function with given data.
```csharp
public abstract void Calculate(GridCalculationData data)
```
| Parameter | Type | Description |
| --- | --- | --- |
| data | GridCalculationData | The required data to calculate function such as function name, parameters, ...etc. |
### Remarks
User should set the calculated value for given data for all functions(including excel native functions) that he wants to calculate by himself in this implementation.
### See Also
* class [GridCalculationData](../../gridcalculationdata/)
* class [GridAbstractCalculationEngine](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

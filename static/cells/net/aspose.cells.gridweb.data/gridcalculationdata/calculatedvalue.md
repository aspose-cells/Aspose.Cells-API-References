##GridCalculationData.CalculatedValue
GridCalculationData property. Gets or sets the calculated value for this function
## GridCalculationData.CalculatedValue property
Gets or sets the calculated value for this function.
```csharp
public object CalculatedValue { get; set; }
```
### Remarks
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property. Getting this property before setting will make the function be calculated by the default calculation engine of Aspose.Cells and the calculated value will be returned.
### See Also
* class [GridCalculationData](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

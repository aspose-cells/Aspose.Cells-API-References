##GridCustomServerValidation.Validate
GridCustomServerValidation method.
## GridCustomServerValidation.Validate method
```csharp
public string Validate(GridWorksheet sheet, int row, int col, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | GridWorksheet | the GridWorksheet |
| row | Int32 | the row index of the cell |
| col | Int32 | the column index of the cell |
| value | String | the value to do validation |
### Return Value
string based result value
### Remarks
if return string.empty the validate is passed,else you can return any related message which can be deal in ClientCallback function
### See Also
* class [GridWorksheet](../../gridworksheet/)
* interface [GridCustomServerValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

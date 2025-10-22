##GridCell.CreateValidation
GridCell method. Creates a validation object for a cell
## GridCell.CreateValidation method
Creates a validation object for a cell.
```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```
| Parameter | Type | Description |
| --- | --- | --- |
| validationType | GridValidationType | Validation type. |
| isRequried | Boolean | Whether the cell value is required. |
### Examples
```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
// Sets to number validation expression.
v.RegEx = "\\d+";
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb()
im sheet As GridWorksheet =  GridWeb1.ActiveSheet
Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True)
' Sets to number validation expression.
v.RegEx = "\\d+"
```
### See Also
* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

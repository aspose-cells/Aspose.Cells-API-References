##WebWorksheet.UpdateBindCellValue
WebWorksheet method. Updates the binding datasource records property value according to the cells value
## WebWorksheet.UpdateBindCellValue method
Updates the binding datasource record's property value according to the cell's value.
```csharp
public void UpdateBindCellValue(GridCell cell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | GridCell | The cell object. |
### Examples
```csharp
cell.PutValue(23.11);
sheet.UpdateBindCellValue(cell);
```
### See Also
* class [GridCell](../../gridcell/)
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

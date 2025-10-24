##GridPivotTable.CalculateData
GridPivotTable method. Calculates pivottables data to cells
## GridPivotTable.CalculateData method
Calculates pivottable's data to cells.
```csharp
public void CalculateData()
```
### Remarks
Cell.Value in the pivot range could not return the correct result if the method is not been called. This method caclulates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.
### See Also
* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

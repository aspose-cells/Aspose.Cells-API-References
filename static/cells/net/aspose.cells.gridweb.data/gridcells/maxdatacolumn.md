##GridCells.MaxDataColumn
GridCells property. Maximum column index of cell which contains data
## GridCells.MaxDataColumn property
Maximum column index of cell which contains data.
```csharp
public int MaxDataColumn { get; }
```
### Remarks
-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.
### See Also
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

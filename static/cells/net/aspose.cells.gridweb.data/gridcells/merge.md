##GridCells.Merge
GridCells method. Merges a specified range of cells into a single cell
## GridCells.Merge method
Merges a specified range of cells into a single cell.
```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
### See Also
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

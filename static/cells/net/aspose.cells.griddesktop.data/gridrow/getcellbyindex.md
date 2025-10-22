##GridRow.GetCellByIndex
GridRow method. Get the cell by specific index in the cells collection of this row
## GridRow.GetCellByIndex method
Get the cell by specific index in the cells collection of this row.
```csharp
public GridCell GetCellByIndex(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index(position) of the cell in the cells collection of this row. |
### Return Value
The Cell object at given position.
### Remarks
To traverse all cells in sequence without modification, using [`GetEnumerator`](../getenumerator/) will give better performance than using this method to get cell one by one.
### See Also
* class [GridCell](../../gridcell/)
* class [GridRow](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

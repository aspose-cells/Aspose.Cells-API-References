##GridWorksheet.GetFreezedPanes
GridWorksheet method. Gets the freeze panes
## GridWorksheet.GetFreezedPanes method
Gets the freeze panes.
```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows,
out int freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32& | Row index. |
| column | Int32& | Column index. |
| freezedRows | Int32& | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32& | Number of visible columns in left pane, no more than column index. |
### Return Value
Return whether the worksheet is frozen
### See Also
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

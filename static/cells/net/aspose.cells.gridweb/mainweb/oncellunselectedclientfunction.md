##MainWeb.OnCellUnselectedClientFunction
MainWeb property. Gets or sets the client side function to be called when a cell is unselected. The client function should be declared like this function MyOnUnselectCellcell  this.setCellValueByCellcell test Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnCellUnselectedClientFunction property
Gets or sets the client side function to be called when a cell is unselected. The client function should be declared like this: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnCellUnselectedClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)

##MainWeb.OnDoubleClickCellClientFunction
MainWeb property. Gets or sets the client side function to be called when a cell is double clicked. The client function should be declared like this function MyOnDoubleClickCellcell  this.setCellValueByCellcell test Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnDoubleClickCellClientFunction property
Gets or sets the client side function to be called when a cell is double clicked. The client function should be declared like this: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnDoubleClickCellClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)

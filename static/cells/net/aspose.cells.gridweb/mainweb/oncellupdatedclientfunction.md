##MainWeb.OnCellUpdatedClientFunction
MainWeb property. Gets or sets the client side function name to be called when a cells value is updated. The client function should be declared like this function MyOnCellUpdatedcell  alertthis.getCellValueByCellcell Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnCellUpdatedClientFunction property
Gets or sets the client side function name to be called when a cell's value is updated. The client function should be declared like this: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnCellUpdatedClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)

##MainWeb.OnCellErrorClientFunction
MainWeb property. Gets or sets the client side function name to be called when a cells validation is failed. The client function should be declared like this function MyOnCellErrorcell  alertthis.getCellValueByCellcell Note You may use the this pointer in the client function to point the grid control which fires the event
## MainWeb.OnCellErrorClientFunction property
Gets or sets the client side function name to be called when a cell's validation is failed. The client function should be declared like this: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
```csharp
public string OnCellErrorClientFunction { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
